pipeline {
  agent any
  stages {
    stage('build for master') {
      when {
        branch 'master'
      }
      steps {
        sh 'echo "this is build stage for master branch"'
        input message: 'Finished using the web site? (Click "Proceed" to continue)'
        sh 'echo ok~'
      }
    }
    stage('build for test') {
      when {
        branch 'test'
      }
      steps {
        sh '''echo "this is build stage for test branch"
pwd'''
      }
    }
  }
}
