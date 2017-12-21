pipeline {
  agent any
  stages {
    stage('build') {
      when {
        branch 'master'
      }
      steps {
        sh '''echo "this is build stage for master branch"
pwd'''
      }
    }
    stage('build') {
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
