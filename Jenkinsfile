pipeline {
    agent any

    stages {

        stage('Checkout') {
            steps {
                git branch: 'master',
                    url: 'https://github.com/Srushtigit09/jenkins_repo.git'
            }
        }

        stage('Deploy') {
            steps {
                sh '''
                echo "Deploying application..."

                 rm -rf /var/www/html/*
                 cp -r * /var/www/html/
                 '''
            }
        }

    }
}
