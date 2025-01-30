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
                withCredentials([string(credentialsId: '14cc424b-d55a-46de-9fa2-3b6de3bd231b', variable: 'mysecret')]) {
                // some block
                echo mysecret
                 }
            }
        }
    }
}
