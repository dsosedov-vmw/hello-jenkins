pipeline {
    agent {
        docker {
            image 'mcr.microsoft.com/windows/nanoserver' //'hello-world'
        }
    }
    //agent any

    stages {
        stage('Build') {
            steps {
                bat 'echo "Hello world"'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}