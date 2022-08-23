pipeline {
    agent {
        kubernetes {
            label 'test-job'
        }
    }

    options {
      buildDiscarder(logRotator(numToKeepStr: '5'))
    }


    stages {
        stage('Checkout') {
            steps {
               script {
                    echo "Hi"
                    sleep(time:5,unit:"SECONDS")
                    echo "bye"
               }
            }
        }
   }
}
