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
                sh 'python3 code.py'  // Agrega Python al PATH
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
