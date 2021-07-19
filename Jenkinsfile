pipeline {
    agent { any { image 'python:3.6.9' } }
    stages {
        stage('build') {
            steps {
                sh 'python --version'
            }
        }
        stage('Linting') { // Run pylint against your code
            steps {
            script {
                sh """pylint main.py"""
        }
      }
    }
    }
}
