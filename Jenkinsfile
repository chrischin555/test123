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
          retry(5){
             echo 'Hello World!'
          }
        }
      }
    }
}
