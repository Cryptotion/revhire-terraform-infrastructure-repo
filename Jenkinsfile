pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git branch: 'main', url: 'https://github.com/david-r-martinez/rev-hire-backend.git'
            }
        }
        stage('Build') {
            steps {
                sh 'terraform init'
                sh 'terraform apply -auto-approve'
            }
        }
        stage('Test') {
            steps {
                sh 'echo "No tests defined yet"'
            }
        }
        stage('Deploy') {
            steps {
                sh 'echo "No deployment defined yet"'
            }
        }
    }
}
