pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
               def username = 'Jenkins'
               echo "I said, Hello Mr. ${username}"
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
               echo "I said, Hello Mr. ${username}"
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
