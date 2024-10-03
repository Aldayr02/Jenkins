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
                sh 'echo $PATH'  // Verifica el PATH disponible en Jenkins
                sh 'where python3'  // Verifica si python3 está en el PATH
                sh 'python3 code.py'  // Ejecuta el script
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
