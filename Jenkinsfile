pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh '''mvn clean compile
'''
        echo 'compilation completed'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn test'
      }
    }
    stage('Deploy') {
      steps {
        sh 'mvn deploy'
      }
    }
  }
}
