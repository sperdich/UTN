pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'git pull https://github.com/sperdich/UTN.git'
        sh 'gradle build'
        sh 'gradle bootRun'
      }
    }

  }
}