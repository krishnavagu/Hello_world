pipeline {
    agent any 
    stages {
        stage('Build') { 
            steps {
                git credentialsId: 'krishna', url: 'https://github.com/krishnavagu/_world.git'
            }
        }
        stage('maven project') { 
            steps {
                sh label: '', script: 'mvn clean package'
            }
        }
        stage('Deploy') { 
            steps {
                echo "this is Deployment"
            }
        }
    }
}
