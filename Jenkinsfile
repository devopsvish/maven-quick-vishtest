pipeline {
    agent second
    
    tools {
        maven "MySlaveMVN"
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
