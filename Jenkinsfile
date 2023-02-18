pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'g++ ./PES2UG20CS912.cpp'
        echo 'Build Stage Successful'
      }
    }
    stage('Test') {
      steps {
        sh './a.out'
        echo 'Test Stage Successful'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deployment Successful'
      }
    }
  }
  post {
      failure {
        echo 'Pipeline Failed'
      }
  }
}
