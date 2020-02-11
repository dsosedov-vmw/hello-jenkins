pipeline {
    agent {
        docker {
            image 'mcr.microsoft.com/dotnet/core/sdk:3.1' //'hello-world'
        }
    }
    //agent any

    stages {
        stage('Build') {
            steps {
            //    sh 'dotnet'
                script {
                    def command = "git --version"
                    def proc = command.execute()
                    proc.waitFor()

                    println "Process exit code: ${proc.exitValue()}"
                    println "Std Err: ${proc.err.text}"
                    println "Std Out: ${proc.in.text}"
                }
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