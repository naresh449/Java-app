ipipeline {
  agent any
  stages {
    stage('Fetch code ') {
      steps {
        git branch:  'master', url:  'https://github.com/naresh449/Java-app.git'
      }
    }
    stage ('build') {
      steps {
        mvnHOME = tool 'mymaven'
        sh "${mvnHOME} install"

      }
    }
    stage ('test') {
      steps {
        sh "${mvnHOME} test"
      }
    }
  }
}
