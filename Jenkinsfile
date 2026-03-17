pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Webhook is working! Pipeline triggered successfully.'
                sh 'echo Repository contents:; ls -la'
            }
        }
    }
    post {
        success { echo 'All good.' }
        failure { echo 'Something went wrong.' }
    }
}
