pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                echo 'Checking out code from Git...'
                git 'https://github.com/<your-username>/<your-repo>.git'
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project...'
                // Example: sh 'mvn clean install' for Java projects
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
                // Example: sh 'mvn test'
            }
        }
    }
}
