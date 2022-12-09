pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build completed'
        retry(count: 3) {
          sh 'cghdhjchc'
        }

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
        input(message: 'Are you sure to deploy?', ok: 'Yes I\'m sure')
        echo 'deployment completed'
      }
    }

    stage('notify for new built') {
      steps {
        echo 'new build completed sucssefuly'
      }
    }

  }
}