pipeline {
    agent any
        environment {
            PATH = "C:\\Users\\Asus\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe"
        }
    stages {
        stage('Checkout Code') {
            checkout scm
        }
        stage('Extract Data') {
            bat "${env.PATH} extract_data.py"
        }
    }
    post {
        success {
            echo "Sucess......"

        }
        failure {
            echo "Failed......"


        }
        always {
            echo "always....."

        }

}