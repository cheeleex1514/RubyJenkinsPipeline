pipeline {
    agent any

stages {
        stage('Build') {
            steps {
                echo '[INFO] Building..'
            }
        }
        stage('Test') {
            steps {
                echo '[INFO] Testing..'
                withMaven() {
                    sh 'mvn -Dtest=ConsoleParserTest test'
                }
            }
        }
        stage('Deploy') {
            steps {
                echo '[INFO] Deploying....'
            }
        }
    }
}