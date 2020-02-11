pipeline {
    agent {
        docker { image 'hello-world' }
    }

    stages {
        stage('Build') {
            steps {
                sh 'echo Hello world'
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