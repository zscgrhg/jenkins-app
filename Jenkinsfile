pipeline {
    agent { docker { image 'nuancemobility/apache-ant' } }



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