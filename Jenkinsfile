pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/lorenguti/IntegracionContinua.git', branch: 'master')
        bat 'gradle build'
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