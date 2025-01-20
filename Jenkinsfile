pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/usuario/proyecto.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }

        stage('Test') {
            steps {
                sh 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Desplegando aplicación...'
            }
        }
    }
}
