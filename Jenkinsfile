pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        sh 'echo "helloWorld"'
        withAWS(region:'us-west-2b', credentials:'aws-static') {
          s3Upload(file:'index.html', bucket:'udacity.devops.project3', path:'/')
        }
      }
    }
  }
}
