pipeline {
    agent {
        docker {
            image 'jenkins/jenkins:lts-jdk17'
            args '-p 3000:3000'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'echo "building"'
                sh 'yarn'
            }
        }
    }
}