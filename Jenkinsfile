pipeline {
  agent {
    node {
      label 'centos'
    }

  }
  stages {
    stage('checkout') {
      steps {
        git(url: 'git@github.com:ktzyl/python-project.git', branch: 'master', credentialsId: '2e0d92a2-ab0c-4bdb-93c6-a79a869e3a04')
      }
    }

    stage('build') {
      steps {
        sh 'python *test.py'
      }
    }

  }
}