node {
  stage('Hello'){
    echo "Hello Worldd!"
  }
}

pipeline {
    agent any
    options {
      timeout(time: 2, unit: 'MINUTES')
    }
    stages{
      stage('Example'){
        steps{
          echo 'Hello World!'
        }
      }
    }
}
