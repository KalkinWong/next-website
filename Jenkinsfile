pipeline {
    agent {
        docker {
            image 'node:16-alpine' 
            args '-p 3000:3000' 
        }
    }
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