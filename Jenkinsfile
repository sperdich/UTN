pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'git pull https://github.com/sperdich/UTN.git'
        sh 'git update-index --chmod=+x gradlew'
        withGradle() {
          sh './gradlew -v'
        }

      }
    }

  }
}