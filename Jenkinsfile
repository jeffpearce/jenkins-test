pipeline {
  agent any
  stages {
    stage ('stage 1') {
      steps {
        sh 'echo stage 1 step 1'
        script {
          if (Math.abs(new Random().nextInt() % 100) < 10) {
            error('fail on purpose');
          }
        }
      }
    }
    stage ('stage 2') {
      steps {
        sh 'echo stage 2 step 1'
        script {
          if (Math.abs(new Random().nextInt() % 100) < 10) {
          error('fail on purpose');
          }
        }
      }
    }
    stage ('stage 3') {
      steps {
        sh 'echo stage 3 step 1'
      }
    }
  }
}
