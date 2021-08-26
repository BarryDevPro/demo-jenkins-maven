pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                
                sh 'mvn -B -DskipTests clean package' 
            }
        }
         stage('Test') {
            steps {
                sh 'mvn test'
            }   
        }
        stage('Run') {
            steps {
                 sh 'cd target/ && java -jar demo-jenkins-1.0-SNAPSHOT.jar'
            }   
        }

    }
}
