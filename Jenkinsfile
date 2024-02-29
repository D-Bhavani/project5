pipeline {
    agent any
    tools {
        node 'node'
    }
    stages {
        stage('checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/D-Bhavani/project5.git'
            }
        }
        stage('install') {
            steps {
                sh 'npm install'
            }
        }
        stage('build') {
            steps {
                sh 'npm run build'
            }
        }
        stage('test') {
            steps {
                sh 'npm test'
            }
        }
    }
}
