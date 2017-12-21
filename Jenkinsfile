pipeline {
  agent any
  stages {
    stage('build for master') {
      when {
        branch 'master'
      }
      steps {
        sh 'ssh -i /home/.ssh/id_rsa 54.223.131.75 "bash /root/test.sh"'
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
