pipeline {
    agent any
    stages {
        stage('Build') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
        }
        stage('run') { 
            steps {
                sh 'java -jar target/demo-jenkins-1.0-SNAPSHOT.jar' 
            }
        }
    }
}
