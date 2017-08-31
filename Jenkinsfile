pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                     
               echo "I said, Hello Mr. ${username}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
               echo "I said, Hello Mr. ${username}"
            }
        }
                stage('Example') {
            steps {
                echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
