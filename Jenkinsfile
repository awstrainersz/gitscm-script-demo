pipeline {
    agent any
    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
        stage('Build') {
            steps {
                withCredentials([string(credentialsId: 'mysecret', variable: 'mysecret')]) {
                // some block
                echo mysecret
                 }
            }
        }
    }
}
