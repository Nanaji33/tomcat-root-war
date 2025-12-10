pipeline {
    agent any
    stages{
        stage("buildcode"){
            steps {
                sh """
                ./mvnw package -Dskiptests
                """    
            }
        }
        
         stage("runtest"){
            steps {
                sh """
                ./mvnw test
                """    
            }
        }
    }
}