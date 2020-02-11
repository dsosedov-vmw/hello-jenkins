pipeline {
    agent {
        docker { image 'hello-world' }
    }

    stages {
        stage('Build') {
            steps {
                sh 'docker run hello-world'
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