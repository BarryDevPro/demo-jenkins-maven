pipeline {
    agent any
    stages {
        stage('Build-run') { 
            steps {
                sh 'mvn -B -DskipTests clean package' 
            }
            steps {
                sh '/var/lib/jenkins/workspace/java-mvn/target/demo-jenkins-1.0-SNAPSHOT.jar' 
            }
        }

    }
}
