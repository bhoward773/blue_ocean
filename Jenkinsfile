pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo '"testing"'
          }
        }

        stage('Parallel') {
          steps {
            echo '"running environment"'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo '"building env"'
      }
    }

    stage('Final') {
      steps {
        echo '"clean up"'
      }
    }

  }
}