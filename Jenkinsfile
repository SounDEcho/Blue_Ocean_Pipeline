pipeline {
  agent any
  stages {
    stage('preprocess') {
      parallel {
        stage('preprocess') {
          steps {
            bat 'echo this is the preprocess stage'
          }
        }
        stage('Kand') {
          steps {
            bat 'echo this is the kand step'
          }
        }
      }
    }
    stage('Compile') {
      steps {
        bat 'echo this is the compile stage'
      }
    }
    stage('Assemble') {
      parallel {
        stage('Assemble') {
          steps {
            bat 'ech this is the assemble stage'
          }
        }
        stage('link') {
          steps {
            bat 'echo this is the link stage'
          }
        }
      }
    }
    stage('Test') {
      steps {
        bat 'echo this is the test stage'
      }
    }
  }
}