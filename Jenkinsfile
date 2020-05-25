pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/lorenguti/IntegracionContinua.git', branch: 'master')
        withGradle()
      }
    }

    stage('Test') {
      steps {
        echo 'Estoy en Test'
      }
    }

    stage('Validate') {
      steps {
        echo 'Estoy en Validate'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Estoy en Deploy'
      }
    }

  }
}