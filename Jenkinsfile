node {

    stage('SCM Checkout') {
        git 'https://github.com/lwemzy/ci-cd.git'
    }

    stage('Compile-Package') {
        environment {
            jdkHome = tool name: 'java-11', type: 'jdk'
        }

        steps {
            sh 'echo $jdkHome'
            sh  'mvn package'
        }
    }
}