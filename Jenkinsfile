pipeline {
    agent { docker { image 'maven:3.3.3' } }
    stages {
        stage('build') {
            steps {
                sh 'echo "Hello World"'
                sh 'mvn --version'
                sh 'mvn package'
            }
        }
    }
}