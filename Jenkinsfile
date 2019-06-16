pipeline {
    agent any
       tools{
        maven 'maven-3.6.1'
    }
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
