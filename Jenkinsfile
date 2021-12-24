node {

    stage('SCM Checkout') {
        git 'https://github.com/lwemzy/ci-cd.git'
    }

    stage('Compile-Package') {
        environment {
            jdkHome = tool name: 'java-11', type: 'jdk'
        }

        
            sh 'echo $jdkHome//usr/lib/jvm/adoptopenjdk-11-hotspot'
            sh  'mvn package'
        
    }
}