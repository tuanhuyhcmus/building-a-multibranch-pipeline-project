pipeline {
    agent {
        docker {
            image 'node:6-alpine'
            args '-p 3000:3000 -p 5000:5000' 
        }
    }
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps{
              echo "ahihi master"
              sh 'pwd'
            }
        
        }
        stage('Test') {
            steps {
               echo "build master done"
            }
        }
    }
}
