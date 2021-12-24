node {
    stage('SCM Checkout') {
        git 'https://github.com/lwemzy/ci-cd.git'
    }

    stage('Compile-Package') {
        sh  'mvn package'
    }
}