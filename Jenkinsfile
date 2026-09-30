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

        stage('Build') {
            steps {
                sh 'echo "Build started"'
                sh 'echo "Building application..."'
                sh 'echo "Build completed successfully"'
            }
        }

        stage('Test') {
            steps {
                sh 'echo "Running tests..."'
                sh 'test -f app.txt'
                sh 'echo "Tests passed"'
            }
        }

        stage('Verify Application') {
            steps {
                sh 'cat app.txt'
            }
        }
    }
}