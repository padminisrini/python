pipeline {
  agent any
  stages {
    stage('checkout') {
      steps {
        git(url: 'https://github.com/padminisrini/python.git', branch: 'main', credentialsId: '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')
      }
    }

    stage('python run') {
      steps {
        sh 'python hello.py'
      }
    }

    stage('echo') {
      steps {
        echo 'Done nice blue ocean'
      }
    }

  }
}