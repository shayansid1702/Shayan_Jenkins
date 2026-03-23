pipeline {
    agent any

    tools {
        maven 'shayan_maven'
    }

    stages {

        stage('Build') {
            steps {
                bat 'mvn clean install'
            }
        }

        stage('Test') {
            steps {
                bat 'mvn test'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying to Tomcat...'
            }
        }
    }
}