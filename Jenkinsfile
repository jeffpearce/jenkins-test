shouldIFail(percentFail) {
  nextRand = Math.abs(new Random().nextInt() % 100)
  print nextRand
  if (nextRand < percentFail) {
    error('fail on purpose');
  }
}

pipeline {
  agent any
  stages {
    stage ('stage 1') {
      steps {
        sh 'echo stage 1 step 1'
        script {
          shouldIFail(25)
        }
      }
    }
    stage ('stage 2') {
      steps {
        sh 'echo stage 2 step 1'
        script {
          shouldIFail(25)
          }
        }
      }
    }
    stage ('stage 3') {
      steps {
        sh 'echo stage 3 step 1'
        script {
          shouldIFail(10)
          }
      }
    }
  }
}
