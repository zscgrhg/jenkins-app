pipeline {
    agent { docker { image 'maven:3.3.3' } }

    environment {

        ANT_HOME    = '${WORKSPACE}/tools/apache-ant-1.10.5-bin/apache-ant-1.10.5/'
        PATH = '${ANT_HOME}/bin:${PATH}'
    }

    stages {
        stage('build') {

            steps {
                  println(WORKSPACE)
                  sh 'echo "Hello World"'

                  sh 'ant build'

            }
        }
    }
}