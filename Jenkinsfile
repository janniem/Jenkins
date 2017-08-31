pipeline {
    def username = 'Jenkins'
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
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
