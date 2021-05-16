pipeline {
  agent any

  stages {
    stage('cleanup') {
      environemnt
      {
          ini i = 10;
      }
      parallel {
        stage('cleanup') {
          steps {
            echo 'Cleanup Completed Stage'
            print i;
          }
        }

        stage('printMessage') {
          steps {
            echo 'parallel Step Execution'
            echo "${env.i}"
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
