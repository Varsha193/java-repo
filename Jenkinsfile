pipeline {
    agent any

    triggers {
        pollSCM('* * * * *')
    }

    stages {
        stage('compile') {
            steps {
                bat 'javac sample.java'
            }
        }

        stage('run') {
            steps {
                bat 'java demo'
            }
        }
    }
}
