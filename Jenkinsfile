 pipeline {
    agent any
    tools {
        maven 'maven-3.9.0'
    }
    stages {
        stage("buildcode") {
            steps {
                sh 'mvn clean package -DskipTests'
            }
        }

        stage("runtest") {
            steps {
                sh 'mvn test'
            }
        }
    }
}
