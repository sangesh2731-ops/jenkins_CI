pipeline {
    agent any
    tools {
        maven 'Maven 3.8.6' // Replace with your configured Maven name in Jenkins Tools
    }
    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com'
            }
        }
        stage('Build') {
            steps {
                sh 'mvn clean package' // Builds the JAR/WAR file
            }
        }
        stage('Test') {
            steps {
                sh 'mvn test' // Runs unit tests
            }
        }
    }
}
