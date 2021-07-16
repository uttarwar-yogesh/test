def test

pipeline {
    agent any
    stages {
        stage('init stage') {
            steps {
                script {
                   test = load "script.groovy" 
                }
            }
        }
    }   
}
