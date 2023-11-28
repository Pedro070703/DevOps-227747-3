pipeline {
    agent any

    stages {
        stage('Check') {
            steps {
                script {
                    checkout scm
                }
            }
        }

        stage('Build TADS') {
            steps {
                script {
                    sh 'npm install'
                    sh 'npm test'
                }
            }
        }
    }
}