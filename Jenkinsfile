pipeline {
  agent any
  stages {
    stage('Fetch code ') {
      steps {
        git branch:  'master', url:  'https://github.com/naresh449/'
      }
    }
    stage ('build') {
      steps {
        sh 'mvn install'

      }
    }
    stage ('test') {
      steps {
        sh 'mvn test'
      }
    }
  }
}
