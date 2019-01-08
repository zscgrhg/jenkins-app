def WORKSPACE = pwd()
def ANT_HOME = '${WORKSPACE}/tools/apache-ant-1.10.5-bin/apache-ant-1.10.5/'
pipeline {
    agent { docker { image 'maven:3.3.3' } }

    environment {

            ANT_HOME = '${WORKSPACE}/tools/apache-ant-1.10.5-bin/apache-ant-1.10.5/'

        }

    stages {
        stage('build') {

            steps {

                  sh 'echo "Hello World"'
                  sh 'echo ${PATH}'
                  sh 'echo ${ANT_HOME}'
                  sh '${ANT_HOME}/ant build'

            }
        }
    }
}