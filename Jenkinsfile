pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
                git url :'https://github.com/Nareshnagar/website.git',branch:'main'
            }
        }

        stage('Build') {
            steps {
                sh 'docker build -t myapp .'
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
