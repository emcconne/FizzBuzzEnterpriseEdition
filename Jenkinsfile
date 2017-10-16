pipeline {
  agent {
    node {
      label 'maven-jdk-8'
    }
    
  }
  stages {
    stage('build') {
      steps {
        sh 'mvn install'
      }
    }
    stage('test') {
      steps {
        sh 'mvn verify'
      }
    }
  }
}