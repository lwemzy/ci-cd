node {
    stage('SCM Checkout') {
        git 'https://github.com/lwemzy/ci-cd.git'
    }

    stage('Compile-Package') {
        // get jdk path
        def jdkHome = tool name: 'java-11', type: 'jdk'
        sh  'mvn package'
    }
}