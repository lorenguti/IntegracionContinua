pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/lorenguti/IntegracionContinua.git', branch: 'master')
        sh './ gradlew build'
      }
    }

    stage('Test') {
      steps {
        echo 'Estoy en Test'
        sh 'ls'
      }
    }

    stage('Validate') {
      steps {
        echo 'Estoy en Validate'
        sh 'ls src'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Estoy en Deploy'
      }
    }

  }
}