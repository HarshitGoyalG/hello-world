pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            echo '"init"'
          }
        }

        stage('Stage3') {
          steps {
            echo '"parallel stage"'
          }
        }

      }
    }

    stage('Stage 2') {
      parallel {
        stage('Stage 2') {
          steps {
            sleep 5
          }
        }

        stage('Stage 4') {
          steps {
            echo 'Parallel Stage 2'
          }
        }

      }
    }

    stage('Stage 5') {
      steps {
        echo '"Final Stage"'
      }
    }

  }
}