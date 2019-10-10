pipeline {
  agent any

  tools {nodejs "nodejs"}

  stages {
    stage('Build') {
      steps {
        sh "npm install"
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
