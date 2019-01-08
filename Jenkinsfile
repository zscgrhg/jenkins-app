pipeline {
    agent { docker { image 'maven:3.3.3' } }

    environment {
            ANT_HOME = '${env.WORKSPACE}/tools/apache-ant-1.10.5-bin/apache-ant-1.10.5/'

        }

    stages {
        stage('build') {
            steps {
                withEnv(['PATH+EXTRA=${ANT_HOME}/bin']) {
                  sh 'echo "Hello World"'
                  sh 'echo ${PATH}'
                  sh 'echo ${ANT_HOME}'
                  sh 'ant build'
                }

            }
        }
    }
}