pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                echo 'Hello World'
                // currentBuild.result == null here
            }
        }
    }
    post {
        always {
            script {
                currentBuild.result = currentBuild.result ?: 'SUCCESS'
                notifyBitbucket()
            }
        }
    }
}
