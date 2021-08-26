pipeline {
    agent any
    stages {
        stage('Build') { 
            steps { 
                sh 'mvn -B -DskipTests clean package' 
                sh 'cd target/ && java -jar demo-jenkins-1.0-SNAPSHOT.jar'
            }
        }
      

    }
}
