pipeline {
  agent any
  stages {
    stage('Compile') {
      steps {
        sh 'cd my-app'
        sh '''mvn clean compile
'''
        echo 'compilation completed'
      }
    }
    stage('Test') {
      steps {
        sh 'cd my-app'
        sh 'mvn test'
      }
    }
    stage('Deploy') {
      steps {
        sh 'cd my-app'
        sh 'mvn deploy'
      }
    }
  }
}
