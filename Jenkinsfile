pipeline {
    agent {
        docker { 
          image 'node:14-alpine'
          args  '-u root:root' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}