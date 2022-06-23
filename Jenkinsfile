pipeline {
  agent any
  stages {
    stage('build') {
      parallel {
        stage('build') {
          steps {
            sh 'echo "1st pipeline in Blue Ocean"'
          }
        }

        stage('test') {
          steps {
            sh 'echo "Parallel Execution"'
          }
        }

      }
    }

    stage('UAT') {
      steps {
        sh 'echo \'Pipeline Complete\''
      }
    }

  }
}