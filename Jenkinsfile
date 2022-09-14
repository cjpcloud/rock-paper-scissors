pipeline {
    agent any

    stages {
        stage('checkout') {
            steps {
                git branch: 'jenkinsfile', credentialsId: '35725a24-eecf-45dc-924a-7a6d41ffb754', url: 'https://github.com/cjpcloud/rock-paper-scissors.git'
            }
        }
	   stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }} 
