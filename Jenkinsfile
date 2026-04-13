pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git 'https://github.com/Nareshnagar/website.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying app...'
            }
        }
    }
}
