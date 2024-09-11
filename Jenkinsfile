pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Clone the Git repository
                git url: 'https://github.com/MurariChukka/newjob.git'
            }
        }
        stage('Deploy') {
            steps {
                // Copy static files to the appropriate directory
                sh '''
                cp -r * /var/www/html/
                '''
            }
        }
    }
}
