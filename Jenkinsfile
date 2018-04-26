
pipeline {
  agent any
    tools {
      gradle "gradle-local"
    }
  stages {
    stage('Build') {
      steps {
        sh 'echo Fase Build;sleep 7;echo Fase Build Terminada'
        sh 'cd ./complete;gradle jar'
      }
    }
    stage('Test'){
      steps {
        sh 'cd ./complete;gradle test'
      }
    }
    stage('Deploy') {
      steps {
        sh 'cd ./complete;gradle installDist'
      }
    }
  }
}

