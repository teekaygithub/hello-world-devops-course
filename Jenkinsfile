pipeline {
    agent any

    tools {
        maven 'maven-3.8.6'
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh "mvn --version"
                sh "mvn clean install"
            }
        }

        stage('Test') {
            steps {
                echo 'Executing unit tests...'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying...'
            }
        }
    }
}