pipeline {
  agent any
  stages {
    stage('Running Java program') {
      steps {
        build 'Writing Code'
        powershell 'javac Hello.java'
        fileExists 'Hello.class'
        powershell(script: 'java Hello', encoding: 'Java Class File')
      }
    }
    stage('Printing the message') {
      steps {
        echo 'Hello World'
      }
    }
  }
}