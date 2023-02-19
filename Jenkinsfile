pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                sh 'g++ -o chaitra pes1ug20cs635.cpp'
                build job : 'PES1UG20CS635-1'
                echo 'Build stage successful'
            }
        }
        stage('Test') {
            steps {
                sh './chaitraa_'
                echo 'Test stage successful'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "Deploying "'
                echo 'Deployment successful'
            }
        }
    }
    post {
        failure {
          echo 'Pipeline failed'
                }
            
        
    }
}
