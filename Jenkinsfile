pipeline {
  agent any
  stages {
    stage('Deployment') {
      steps {
        echo 'Build identified for deployment'
      }
    }

    stage('check DO setup health') {
      steps {
        waitUntil(initialRecurrencePeriod: 3, quiet: true) {
          isUnix()
        }

      }
    }

  }
}