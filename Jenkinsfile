pipeline {
    agent {
        docker {
            image 'hello-world'
            args '-i'
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