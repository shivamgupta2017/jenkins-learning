pipeline {
    // agent {
    //     docker { 
    //       image 'node:14-alpine'
    //       args  '-u C:C' }
    // }
    stages {
        stage('Test') {
            input {
                message "Should we continue?"
                ok "Yes, we should."
                submitter "alice,bob"
                parameters {
                    string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')
                }
            }
            steps {
                echo "Hello, ${PERSON}, nice to meet you."
            }
        }
    }
}