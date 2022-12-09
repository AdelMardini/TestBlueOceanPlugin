pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
      }
    }

    stage('Test Stages') {
      parallel {
        stage('Test Stages') {
          steps {
            echo 'test2'
          }
        }

        stage('Test1') {
          steps {
            echo 'running test1'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deployment completed'
      }
    }

  }
}