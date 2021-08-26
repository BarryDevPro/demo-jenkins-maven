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
                sh '/var/lib/jenkins/workspace/java-mvn/target/demo-jenkins-1.0-SNAPSHOT.jar' 
            }
        }
    }
}
