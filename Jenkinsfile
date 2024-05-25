pipeline {
    agent any
    // Définition de l'environnement Node.js
    tools {
        nodejs "TestNode"
    }

    stages {
        stage('Build') { 
            steps {
                sh 'npm install' 
            }
        }
    stage('Test') {
            steps {
                sh './jenkins/scripts/test.sh'
            }
        }
    }

}
