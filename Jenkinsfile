pipeline {
  agent {
    docker {
      args '-e TZ="Asia/Taipei"'
      image 'lancechienli12/btqav2'
    }

  }
  stages {
    stage('Checkout') {
      steps {
        git(url: 'https://gitlab01.oa.btse.io/btse/btse-qa/pytest_allure.git', branch: 'master', changelog: true, credentialsId: 'GitKey-Lance')
      }
    }

  }
}