pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/Anusha156-code/python-jenkins-demo.git'
            }
        }
        stage('Run Python Script') {
            steps {
                bat 'python --version'   // ✅ prints Python version first
                bat 'python index.py'    // ✅ runs your script
            }
        }
        stage('Run Tests') {
            steps {
                bat 'pytest'
            }
        }
        stage('Lint') {
            steps {
                bat 'flake8 .'
            }
        }        
    }
}
