pipeline {
    agent any
    tools {
        maven 'maven'
    }
       
    stages {
        stage('maven clean'){
            steps {
                sh 'mvn clean'
            }
        }
        stage('maven compile'){
            steps {
                sh 'mvn compile'
            }
        }
        stage('maven package'){
            steps {
                sh 'mvn package'
            }
        }     
    }
    post {
        success {
            echo 'its working good'
        }
        failure {
            echo 'its not working'
        }
    }
}
