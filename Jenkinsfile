pipeline {
    agent any
    stages {
        stage('No-op') {
            steps {
                sh 'ls'
            }
        }
    }
    post {
        always {
            echo 'One way or another, I have finished'
            deleteDir() /* clean up our workspace */
        }
        success {
        mail to: 'jan.niemietz@traveltainment.de',
             subject: "Pipeline succeeded: ${currentBuild.fullDisplayName}",
             body: "${env.BUILD_URL} kicked butt!"
        }
        unstable {
            echo 'I am unstable :/'
        }
        failure {
        mail to: 'jan.niemietz@traveltainment.de',
             subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
             body: "Something is wrong with ${env.BUILD_URL}"
        }
        changed {
            echo 'Things were different before...'
        }
    }
}
