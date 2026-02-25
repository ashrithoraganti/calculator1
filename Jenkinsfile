pipeline {
  agent any
  stages {
    stage('clone') {
      steps {
        git branch:'main' url:'https://github.com/ashrithoraganti/calculator1.git';
      }
    }
    stage('compile') {
      steps {
        sh 'javac Calculator1.java'
      }
    }
    stage('build') {
      steps {
        sh 'java Calculator1 25 5'
      }
    }
    stage('test') {
      steps {
        sh 'java Calculator1 30 -5'
  }
  }
    stage('deploy') {
      steps {
        echo 'deployment completed'
      }
    }
  }
}
