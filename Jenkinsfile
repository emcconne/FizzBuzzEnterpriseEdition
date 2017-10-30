pipeline {
  agent {
    docker {
      image 'maven'
    }
    
  }
  stages {
    stage('Compile') {
      steps {
        sh 'mvn clean package'
      }
    }
    stage('Test') {
      steps {
        sh 'mvn verify'
      }
    }
  }
}