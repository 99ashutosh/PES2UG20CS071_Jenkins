pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'make'
        echo 'Build Successful'
      }
    }
    stage('Test') {
      steps {
        sh '/var/jenkins_home/workspace/PES2UG20CS071-1/hello_exec'
      }
    }
  }
  post {
    failure {
      echo 'Task Failed'
    }
  }
}
