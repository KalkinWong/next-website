pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'echo "Building - start install"'
                sh 'npm install' 
            }
        }
    }
    post {
        always{
            steps{
                echo 'always'
            }
        }
    }
}