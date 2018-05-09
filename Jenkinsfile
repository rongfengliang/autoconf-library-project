pipeline {
  agent {
    node {
      label 'docker-64'
    }

  }
  stages {
    stage('autoconf build') {
      steps {
        sh './autogen.sh'
      }
    }
    stage('configure') {
      steps {
        sh './configure'
      }
    }
    stage('make') {
      steps {
        sh 'make'
      }
    }
  }
}
