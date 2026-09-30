pipeline {
    agent {
        label 'linux-agent'
    }

    stages {
        stage('Verify Agent') {
            steps {
                sh 'hostname'
                sh 'whoami'
                sh 'java --version'
            }
        }

        stage('Verify Application') {
            steps {
                sh 'cat app.txt'
            }
        }
    }
}
