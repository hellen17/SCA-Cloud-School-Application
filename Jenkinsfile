pipeline {
    agent { any { image 'python:3.6.9' } }
    stages {
        stage('build') {
            steps {
                sh 'python main.py'
            }
        }
        stage('Linting') { // Run pylint against your code
            steps {
            script {
                sh """pylint main.py --disable=missing-docstring"""
        }
      }
    }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
