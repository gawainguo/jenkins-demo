pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage('build') {
            steps {
                echo 'hi build'
                sh 'mvn clean package -DskipTests'

            }
        }
        stage('health-check') {
            steps {
                echo 'hi health-check'
            }
        }
    }
}