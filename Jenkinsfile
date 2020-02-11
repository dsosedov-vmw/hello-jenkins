pipeline {
    agent {
        docker {
            image 'mcr.microsoft.com/dotnet/core/sdk:3.1' //'hello-world'
        }
    }
    //agent any

    stages {
        stage('Build') {
            //steps {
            //    sh 'dotnet'
            //}
            script {
                def sout = new StringBuilder(), serr = new StringBuilder()
                def proc = 'ls /badDir'.execute()
                proc.consumeProcessOutput(sout, serr)
                proc.waitForOrKill(1000)
                println "out> $sout err> $serr"
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