pipeline {
    agent ak_slave 
    stages {
        stage('Build') { 
            steps {
              sh "mvn clean"
            }
        }
        stage('Test') { 
            steps {
               sh "mvn test"
            }
        }
        stage('package') { 
            steps {
                sh " mvn test" 
            }
        }
        stage('deploy'){
            steps{
              echo "deploy to tomcat server on ec2"   
            }
        }
    }
}
