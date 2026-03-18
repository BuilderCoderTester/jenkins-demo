pipeline {
    agent any

    tools {
        nodejs 'Node-18'
    }

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/BuilderCoderTester/jenkins-demo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                bat 'npm install'
            }
        }

        stage('Build') {
            steps {
                bat 'npm run build'
            }
        }
    }
}
