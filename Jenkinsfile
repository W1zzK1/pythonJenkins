pipeline {
    agent any

    stages {
        stage('Setup') {
            steps {
                script {
                    // Установите Python, если он еще не установлен
                    sh 'sudo apt-get update'
                    sh 'sudo apt-get install -y python3'
                }
            }
        }

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
