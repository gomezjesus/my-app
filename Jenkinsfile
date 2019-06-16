pipeline {
    agent any 
    stages {
         stage('---cleanWorkspace---') {
            steps {
                cleanWs()
            }
        }
        stage('---test---') { 
            steps {               
                sh "mvn test"
            }
        }
        stage('---package---') { 
            steps {
                sh "mvn package" 
            }
        }
    }
}
