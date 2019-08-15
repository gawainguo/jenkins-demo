pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('build') {
            steps {
                echo 'hi build'
            }
        }
        stage('health-check') {
            steps {
                echo 'hi health-check'
            }
        }
    }
}