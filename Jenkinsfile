pipeline {
    agent {
        docker {
            image 'node:16.15.0-alpine3.14' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'chmod 744 ./jenkins/scripts/build.sh'
                sh './jenkins/scripts/build.sh'
            }
        }
    }
}