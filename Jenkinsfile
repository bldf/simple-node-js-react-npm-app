pipeline {
    agent {
        docker {
            image 'node:17.7.2' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh './jenkins/scripts/build.sh'
            }
        }
    }
}