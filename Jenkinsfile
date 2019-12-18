pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
              sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
               sh "mvn package"
            }
        }
        stage('Deploy') { 
            steps {
                sh " echo deploying to tomcats" 
            }
        }
    }
}
