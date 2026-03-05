pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/AA2543/carwebsite.git'
            }
        }

        stage('Deploy to Apache') {
            steps {
                sh 'sudo cp -r * /var/www/html/'
            }
        }
    }
}

