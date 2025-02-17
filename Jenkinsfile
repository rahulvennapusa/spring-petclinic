pipeline {
    agent any
    tools {
        maven 'MAVEN_HOME'
    }


    stages {

        stage('clean') {
            steps {
                echo 'maven clean...'
                // Add your clean steps here
                sh 'mvn clean'
            }
        }
        stage('Build') {
            steps {
                echo 'Building...'
                // Add your build steps here
                sh 'mvn compile'
                sh 'mvn package'
                	

            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                // Add your test steps here
                sh 'mvn test'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                // Add your deploy steps here
                sh 'mvn deploy'
            }
        }
    }
}
