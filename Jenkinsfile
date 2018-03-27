pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh 'echo "This is the compile step"'
      }
    }
    stage('UnitTest') {
      parallel {
        stage('UnitTest') {
          steps {
            sh 'echo "This is the Unit test"'
          }
        }
        stage('UITest') {
          steps {
            sh 'echo "This is the UI test"'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "This is the deploy step"'
      }
    }
  }
}