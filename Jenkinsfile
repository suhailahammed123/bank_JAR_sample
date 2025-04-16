pipeline {
  agent {
    label 'java_slave_node'
  }

  tools {
    maven 'maven'
  }

  stages {
    stage("prepare the build") {
      steps {
        sh 'mvn clean package'
      }
    }
  }
}
