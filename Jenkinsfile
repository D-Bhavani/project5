pipeline {
    agent any
    tools {
        // Define Node.js and npm installations
        nodejs 'node'
    }

    stages {
        stage('Checkout') {
            steps {
                // Checkout your code from version control
                git branch: 'main', url: 'https://github.com/D-Bhavani/project5.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'npm install'
            }
        }

        stage('Build') {
            steps {
                // Build React application
                sh 'npm run build'
            }
        }

        stage('Test') {
            steps {
                // Run tests
                echo 'npm test'
            }
        }
    }
}
