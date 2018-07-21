pipeline {
  agent any
  stages {
    stage('Running Java program') {
      steps {
        sh 'javac hello.java'
        fileExists 'Hello.class'
        powershell(encoding: 'UTF-8', script: 'javac hello.java', returnStdout: true, returnStatus: true)
      }
    }
    stage('Printing the message') {
      steps {
        echo 'Hello World'
      }
    }
  }
}