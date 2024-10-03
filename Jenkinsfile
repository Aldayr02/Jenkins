pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                checkout scm
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'sudo cat code.py'  // Usar python3 del PATH
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
