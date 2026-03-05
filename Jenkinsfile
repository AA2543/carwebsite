pipeline {
    agent any

    stages {

        stage('Checkout Code') {
            steps {
                git branch: 'master', 
                url: 'https://github.com/AA2543/carwebsite.git'
            }
        }

        stage('Deploy to Apache') {
            steps {
                sh '''
                    rm -rf /var/www/html/*
                    cp -r * /var/www/html/
                ''' 
            }
        }

      post {
        success {
          echo 'Website Deployed Successfully!'
        }
        failure {
          echo 'Deployment failed!'
        }
      }

     

    }
}

