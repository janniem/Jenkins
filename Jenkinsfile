pipeline {
    agent any
    stages {
        /* "Build" and "Test" stages omitted */

        stage('Sanity check') {
            steps {
                input "Does the staging environment look ok?"
            }
        }

        stage('Deploy - Production') {
            steps {
                echo 'success'
            }
        }
    }
}
