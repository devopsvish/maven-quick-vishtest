pipeline {
    agent {
        label "node-1"
    }

    tools {
        maven "MySlaveMVN2"
    }

    stages {
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
