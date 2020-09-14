pipeline {
  agent any
  stages {
    stage('print') {
      steps {
         git 'https://github.com/Dgotlieb/JenkinsTest.git'
      }
    }
    stage('print2') {
      steps {
        bat 'python 1.py'
      }
    }
  }
}
