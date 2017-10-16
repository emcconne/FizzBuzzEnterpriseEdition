pipeline {
  agent {
    docker {
      image 'maven'
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