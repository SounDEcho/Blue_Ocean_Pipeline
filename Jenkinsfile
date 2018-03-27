pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        echo 'This is a compile step'
      }
    }
    stage('UITest') {
      parallel {
        stage('UITest') {
          steps {
            echo 'This is the UI test'
          }
        }
        stage('UnitTest') {
          steps {
            echo 'This is the unit test'
          }
        }
      }
    }
    stage('Deploy') {
      steps {
        echo 'this is the deploy stage'
      }
    }
  }
}