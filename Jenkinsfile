pipeline {
    agent any

    tools {
        maven 'maven'
    }

    stages{
        stage("clean") {
            steps{
                sh 'mvn clean'
            }
            post {
                success {
                    echo "cleaning is successfull"
                }
                failure {
                    echo "cleaning is failure"
                }
            }
        }
        stage("validate"){
            steps{
                sh 'mvn validate'
            }
            post {
                always {
                    echo "always execute"
                }
                success{
                    echo "validate is successfull"
                }
                failure {
                    echo "validate is failure"
                }
            }
        }
        stage("package"){
            steps {
                sh 'mvn package'
            }
        }
    }
    post {
        always {
            echo "pipeline executed"
        }
        success {
            echo "its successfully completed"
        }
        failure {
            echo "pipeline failure"
        }
    }
}
