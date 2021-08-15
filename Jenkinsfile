pipeline {
    agent {
        docker { 
          image 'node:14-alpine'
          args  '-u C:C' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}