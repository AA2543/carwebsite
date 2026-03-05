pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/AA2543/carwebsite.git'
            }
        }

        stage('Deploy') {
            steps {
                sh 'cp -r * /var/www/html/'
            }
        }
    }
}

