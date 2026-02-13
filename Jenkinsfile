pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                checkout scm
            }
        }

        stage('Copy to Target Folder') {
            steps {
                sh '''
                rm -rf /var/www/dev-app/*
                cp -r * /var/www/dev-app/
                '''
            }
        }
    }
}

