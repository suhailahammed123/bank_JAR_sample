pipeline {
  agent any

  stages {
    stage("print server info") {
      steps {
        echo "hello devops"
        sh """
            echo $JOB_NAME
            echo $BUILD_ID
            uptime
            whoami
            pwd
            echo $HOSTNAME
          """
      }
    }
  }
}
