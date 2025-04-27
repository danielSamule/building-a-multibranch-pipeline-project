pipeline {
    agent any
    environment {
        CI = 'true'
    }
    stages {
        stage('Build') {
            steps {
                sh 'npm install'
            }
        }
        stage('Grow') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
    }
}