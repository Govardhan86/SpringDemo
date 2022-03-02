pipeline {
    agent any
    tools{
        maven 'MAVEN' 
        jdk 'JAVA'
    }
    stages {
        stage('Git Checkout') {
            steps {
                git 'https://github.com/Govardhan86/SpringDemo.git'
            }
        }
        stage('Build') {
            steps {
                echo 'Building ...'
                bat 'mvn clean package'
                
            }
        }
        stage('Test') {
            steps {
                echo 'Testing the project'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying the project'
            }
        }
        }
    }
