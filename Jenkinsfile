pipeline {
  agent any
  stages {
    stage ('checkout') {
      steps {
        git 'https://github.com/laxmagithub/maven-project.git';
      }
    }
    stage ('Build') {
      steps {
        bat 'mvn clean'
      }
    }
    stage('Unit Test') {
        steps {
            mvn 'test'
        }
    }
  }
