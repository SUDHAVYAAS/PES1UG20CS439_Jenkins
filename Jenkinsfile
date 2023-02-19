pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'g++ error -o error'
                 build job: 'PES1UG20CS439-1', wait: false
                 echo 'Build by CS439 successful'
            }
        }

        stage('Test') {
            steps {
                sh 'cat temp.cpp'
                echo 'Test by CS439 successful'
            }
        }

        stage('Deploy') {
            steps {
               
                echo 'Deploy by CS439 successful'
            }
        }
    }

    post {
        failure {
            
                echo 'Pipeline Failed'
          
        }
    }
}
