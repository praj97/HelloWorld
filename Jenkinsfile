pipeline {
  agent any
  stages {
    stage('Running Java program') {
      steps {
        sh 'javac hello.java'
        fileExists 'Hello.class'
        sh 'java Hello'
      }
    }
    stage('Printing the message') {
      steps {
        echo 'Hello World'
      }
    }
  }
}