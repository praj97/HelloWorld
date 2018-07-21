pipeline {
  agent any
  stages {
    stage('Running Java program') {
      steps {
        sh 'javac hello.java'
        fileExists 'Hello.class'
      }
    }
    stage('Printing the message') {
      steps {
        echo 'Hello World'
      }
    }
  }
}