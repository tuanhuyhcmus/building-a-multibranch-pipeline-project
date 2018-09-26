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
              echo "ahuhu"
              echo "ahihi master"
              sh 'pwd'
            }
        
        }
        stage('Deliver for development') {
            when {
                branch 'development'
            }
            steps {
               echo "Deliver for development success "
            }
        }
        stage('Deploy for production') {
            when {
                branch 'production'
            }
            steps {
               echo "Deploy for production success"
            }
        }
        stage('Build for master') {
            when {
                branch 'master'
            }
            steps {
               echo "Build for master success"
            }
        }
    }
}
