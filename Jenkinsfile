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
                sh 'python3 index.py'
            }
        }
    }
}
