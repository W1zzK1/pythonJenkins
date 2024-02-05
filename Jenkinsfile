pipeline {
    agent {
        docker {
            image 'python:3.8-slim'
        }
    }
    stages {
        stage('Run Python code') {
            steps {
                script {
                    // Запустите ваш Python код
                    sh 'python3 main.py'
                }
            }
        }
    }
}
