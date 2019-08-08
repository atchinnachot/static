pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh 'echo "helloWorld"'
        sh '''
          echo "Multiline shell steps works too"
          ls -lah
         '''
      }
    }
  }
}