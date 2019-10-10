pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        npm run build:prod
        npm run test:ci
      }
    }

    stage('Deploy') {
      steps {
        npm run deploy
      }
    }
  }
}
