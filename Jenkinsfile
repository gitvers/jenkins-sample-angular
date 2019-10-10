pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        sh "npm run build:prod"
        sh "npm run test:ci"
      }
    }

    stage('Deploy') {
      steps {
        sh "npm run deploy"
      }
    }
  }
}
