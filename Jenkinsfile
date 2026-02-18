pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Compiling HelloJenkins...'
                bat 'javac HelloJenkins.java'
            }
        }

        stage('Archive') {
            steps {
                echo 'Archiving artifact...'
                archiveArtifacts 'HelloJenkins.class'
            }
        }

        stage('Run') {
            steps {
                echo 'Running program...'
                bat 'java HelloJenkins'
            }
        }
    }
}
