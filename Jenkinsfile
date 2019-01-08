pipeline {
    agent { docker { image 'maven:3.3.3' } }

    environment {
            def WORKSPACE = pwd()
            ANT_HOME = '${WORKSPACE}/tools/apache-ant-1.10.5-bin/apache-ant-1.10.5/'

        }

    stages {
        stage('build') {
            def WORKSPACE = pwd()
            def ANT_HOME = '${WORKSPACE}/tools/apache-ant-1.10.5-bin/apache-ant-1.10.5/'
            steps {

                  sh 'echo "Hello World"'
                  sh 'echo ${PATH}'
                  sh 'echo ${ANT_HOME}'
                  sh '${ANT_HOME}/ant build'

            }
        }
    }
}