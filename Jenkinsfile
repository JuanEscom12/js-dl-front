pipeline {
  agent {
    docker { image 'node:latest' }
  }
  stages {
    stage('Install') {
      steps { sh 'npm install' }
    }

    stage('Test') {
      parallel {
        stage('Static code analysis') {
            
        }
        stage('Unit tests') {
           
        }
      }
    }

    stage('Build') {
      steps { sh 'npm run-script build' }
    }
  }
}