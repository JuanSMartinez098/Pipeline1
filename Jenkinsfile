pipeline {
  agent any
  stages {
    stage('Paso1') {
      parallel {
        stage('Paso1') {
          steps {
            build 'PROYECTO-MAVEN'
          }
        }

        stage('Paso1.1') {
          steps {
            build 'JOB1'
          }
        }

      }
    }

    stage('Paso2') {
      steps {
        build 'JOB3'
      }
    }

    stage('Paso3') {
      steps {
        build 'TomcatPruebas'
      }
    }

  }
}