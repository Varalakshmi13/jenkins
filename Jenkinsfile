pipeline {
  agent any

  environment {
    ENV_URL = "pipeline.google.com"
  }
  stages {

    stage('One') {
      steps{
        echo "One"
        sh 'echo ENV_URL = ${ENV_URL}'
      }
    }
    stage('Two') {
      steps{
        echo "Two"
      }
    }
  }

}