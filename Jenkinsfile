pipeline {
  agent any

script 
{
public int i = 10;

}

  stages {
    stage('cleanup') {
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
