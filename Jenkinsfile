pipeline {
  agent any
    parameters {
        string(name: 'ENVIRONMENT', defaultValue: 'development', description: '')
    }
  stages {
    stage ('stage 1') {
        environment {
            DEPLOYMENT = "DEVELOPMENT"
        }
      steps {
        sh 'echo stage 1 step 1'
      }
    }
    stage ('stage 2') {
      steps {
        sh 'echo stage 2 step 1'
        cobertura coberturaReportFile: '*.xml'

      }
    }
  }
}
