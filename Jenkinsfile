pipeline {
    agent {
        any {
            image 'maven:3-alpine' 
            args '-v C:\apache-maven-3.6.3\bin' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                bat 'mvn -B -DskipTests clean package' 
            }
        }
    }
}
