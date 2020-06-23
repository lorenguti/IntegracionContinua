pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        git(url: 'https://github.com/lorenguti/IntegracionContinua.git', branch: 'master')
        sh 'chmod +x gradlew'
        sh './gradlew build'
      }
    }

    stage('Test') {
      steps {
        echo 'Estoy en Test'
        sh 'ls gradle'
      }
    }

    stage('Validate') {
      steps {
        echo 'Estoy en Validate'
        sh 'ls gradlew'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Estoy en Deploy'
        sh 'chmod +x gradle'
        sh './gradle/wrapper/gradle-wrapper.jar'
      }
    }

  }
}