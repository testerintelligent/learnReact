pipeline {
  agent any
  stages {
    stage('cleanup') {
      parallel {
        stage('cleanup') {
          steps {
            echo 'Cleanup Completed'
          }
        }

        stage('printMessage') {
          steps {
            echo 'parallel Step Execution'
          }
        }

      }
    }

    stage('nextStage') {
      steps {
        echo 'secondStage'
      }
    }

  }
}