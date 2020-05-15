pipeline {
  agent any
  stages {
    stage('View env') {
      steps {
        sh 'env'
      }
    }
    stage('Test') {
      steps {
        sh 'cat code | grep -i "Continuous integration is great!"'
        sh '[ $(ls | wc -l) -ge 3 ]'
      }
    }

  }
}
