pipeline {
    agent any
       tools{
        maven 'maven-3.6.1'
    }
    stages {
         stage('---clean---') {
            steps {
                sh "mvn clean"
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
