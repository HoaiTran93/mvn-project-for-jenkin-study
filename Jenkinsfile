pipeline {
    agent any 
    stages {
        stage('Clone and Clean maven project') { 
            steps {
                sh "/usr/local/bin/mvn clean"
            }
        }
        stage('Test') { 
            steps {
                sh "/usr/local/bin/mvn test"
            }
        }
        stage('Deploy') { 
            steps {
                sh "/usr/local/bin/mvn package"
            }
        }
    }
}