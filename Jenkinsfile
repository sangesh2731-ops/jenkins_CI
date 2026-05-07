pipeline {
    agent any
    stages {
        stage('Checkout') {
            steps {
                // Manually tell Jenkins which repo to clone
                git 'https://github.com'
            }
        }
        stage('Compile') {
            steps {
                bat 'javac App.java' 
            }
        }
        stage('Run') {
            steps {
                bat 'java App'
            }
        }
    }
}
