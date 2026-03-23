pipeline {
    agent any

    tools {
        maven 'shayan_maven'
    }

    stages {

        stage('Clone') {
            steps {
                git 'https://github.com/shayansid1702/Shayan_Jenkins'
            }
        }

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