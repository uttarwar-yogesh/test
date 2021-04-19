def test

pipeline {
    agent any
    stages {
        stage('init') {
            steps {
                script {
                   test = load "script.groovy" 
                }
            }
        }
    }   
}
