pipeline {
  agent any

  options {
      enforceBuildSchedule()
  }

  stages {
    stage ('stage 1') {
      steps {
        sh 'echo stage 1 step 1'
      }
    }
    stage ('stage 2') {
      steps {
        sh 'echo stage 2 step 1'
      }
    }
    stage ('stage 3') {
      steps {
        sh 'echo stage 3 step 1'
      }
    }
  }
}
