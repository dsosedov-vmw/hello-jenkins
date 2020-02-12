pipeline {
    agent {
        docker {
            image 'hello-world'
        }
    }

    stages {
        stage('Build') {
            steps {
                bat 'dotnet'
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
