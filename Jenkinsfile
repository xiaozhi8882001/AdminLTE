pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            build(job: 'job1', propagate: true, quietPeriod: 1)
          }
        }
        stage('step2') {
          steps {
            powershell 'echo \'ss\''
          }
        }
      }
    }
  }
}