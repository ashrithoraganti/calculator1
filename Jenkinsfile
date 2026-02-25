pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        git branch:'main',url:'https://github.com/ashrithoraganti/calculator1.git';
      }
    }
    stage('compile') {
      steps {
        sh 'javac calculator1.java'
      }
    }
    stage('build') {
      steps {
        sh 'java calculator1 25 5'
      }
    }
    stage('test') {
      steps {
        sh 'java calculator1 30 -5'
  }
  }
    stage('deploy') {
      steps {
        echo 'deployment completed'
      }
    }
  }
}
