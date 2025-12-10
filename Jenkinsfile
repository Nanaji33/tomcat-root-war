 pipeline {
    agent any
    tools {
        maven 'Maven-3.9'
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
