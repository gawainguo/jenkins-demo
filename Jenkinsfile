pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
        stage('build') {
            steps {
                sh 'mvn clean instal -DskipTest'
            }
        }
        stage('health-check') {
            steps {
                sh 'curl http://localhost:8000/health'
            }
        }
    }
}