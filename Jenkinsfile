pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh '/opt/homebrew/bin/mvn clean compile'
            }
        }

        stage('Test') {
            steps {
                echo 'Testing...'
                sh '/opt/homebrew/bin/mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
                sh 'echo Deployment Successful!'
            }
        }
    }
}