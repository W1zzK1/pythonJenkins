pipeline {
    agent {
        docker {
            image 'python:3.12.1-alpine3.19'
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
