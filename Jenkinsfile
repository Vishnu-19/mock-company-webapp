pipeline {
    agent any
    tools {
        maven 'maven'
        jdk 'jdk11'
    }
    stages {
        stage('Test') {
            steps {
                sh './gradlew test'
            }
        }
        stage('Build') {
            steps {
                sh './gradlew assemble'
            }
        }
    }
}
