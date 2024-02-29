pipeline {
    agent any

    tools node:node

    stages('checkout') {
        stage {
            steps {
                git branch: 'main', url: 'https://github.com/D-Bhavani/project5.git'
            }
        }
    }

    stage('npminstall') {
        steps {
            sh 'npm install'
        }
    }
    stage('build') {
        steps {
            sh 'npm run build'
        }
    }
}
