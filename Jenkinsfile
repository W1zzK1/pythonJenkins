pipeline {
    agent {
        docker {
            image 'alpine'
        }
    }
    stages {
        stage('Setup') {
            steps {
                sh 'apk add --no-cache python3 && ln -sf python3 /usr/bin/python'
                sh 'python --version'
            }
        }
        stage('version') {
            steps {
                sh 'python3 --version'
            }
        }
        stage('build') {
            steps {
                sh 'python3 main.py'
            }
        }
    }
}
