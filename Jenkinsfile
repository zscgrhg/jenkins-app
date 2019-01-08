pipeline {
    agent { docker { image 'maven:3.3.3' } }



    stages {
        stage('build') {

            steps {

                  sh 'echo "Hello World"'

                  sh './tools/apache-ant-1.10.5-bin/apache-ant-1.10.5/ant build'

            }
        }
    }
}