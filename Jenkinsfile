pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                git 'https://github.com/Godwin4321/ci-cd-assignment.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'python3 -m pip install --upgrade pip'
            }
        }

        stage('Run Tests') {
            steps {
                sh 'python3 -m unittest discover'
            }
        }
    }
}
