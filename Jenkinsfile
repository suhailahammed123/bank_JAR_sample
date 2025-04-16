pipeline {
  agent any

  stages {
    stage("print server info") {
      steps {
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
