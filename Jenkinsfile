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
            post {
                always {
                    java  '-jar target/demo-jenkins-1.0-SNAPSHOT.jar'
                }
            }
        }

    }
}
