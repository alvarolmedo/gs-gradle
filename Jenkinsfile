
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
sh 'pwd'
}
}
stage('Deploy') {
steps {
sh 'echo Fase Deploy;sleep 10;echo Fase Test Deploy'
}
}
}
}

