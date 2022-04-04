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
      environment {
        ENV_URL = "stage.google.com"
      }
      steps{
        echo "Two"
        sh 'echo ENV_URL = ${ENV_URL}'
        sh 'env'
        sh '''
          echo -e "\\e[31mHello]"
        '''
      }
    }
  }

}