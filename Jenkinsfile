pipeline {
    agent any
    triggers {
  pollSCM '* * * * *'
    }
    tools {
        maven 'M2_HOME' 
    }
    stages {
        stage('Hello') {
            steps {
                sh 'docker ps'
                sh 'docker images'
                echo 'Hello World'
                sleep 10
            }
         
            
        }
    

    
        stage('Rodrigue') {
            steps {
                echo 'Rodrigue World'
                sleep 10 
            }
        }
    

    stage('Maven') {
            steps {
                echo 'Maven World'
                sh 'mvn --version'
            }   sh ' mvn test'
        }       sh 'mvn clean'
                sh 'mvn install'
                sh 'mvn package'
            
        stage('Succes') {
            steps {
                echo 'Succes World'
            }
        }
    }

   

}