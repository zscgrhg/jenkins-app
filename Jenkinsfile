pipeline {
    agent { docker { image 'maven:3.3.3' } }

    environment {
            ANT_HOME = '${env.WORKSPACE}/tools/apache-ant-1.10.5-bin/apache-ant-1.10.5/'
            PATH+EXTRA ='${env.ANT_HOME}/bin'
        }

    stages {
        stage('build') {
            steps {
                sh 'echo "Hello World"'
                sh 'ant build'
            }
        }
    }
}