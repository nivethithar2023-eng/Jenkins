pipeline {
    agent any

    stages {

        stage('Build') {
            steps {
                echo 'Compiling HelloJenkins...'
                sh 'javac HelloJenkins.java'
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
                sh 'java HelloJenkins'
            }
        }
    }
}
