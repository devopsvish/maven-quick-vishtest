pipeline {
    agent any
    
    tools {
        maven "maven-3.9.5"
    }

    stages {
        stage('Git Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/devopsvish/maven-quick-vishtest.git'
            }
        }
        
        stage('mvn compile') {
            steps {
                sh 'mvn compile'
            }
        }
        
        stage('mvn package') {
            steps {
                sh 'mvn package'
            }
        }
        
        stage('mvn install') {
            steps {
                sh 'mvn install'
            }
        }
    }
}
