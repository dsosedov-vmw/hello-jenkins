pipeline {
    agent {
        docker { image 'hello-world:nanoserver' }
    }

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