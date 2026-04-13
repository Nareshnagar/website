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
                bat 'pip install -r requirements.txt'

                bat 'docker build -t myapp .'
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
                bat 'docker run -d -p 8000:8000 myapp'
                echo 'Deploying app...'
            }
        }
    }
}
