node {
  stage('Hello'){
    echo "Hello Worldd!"
  }
}

pipeline {
    agent {
        docker { image 'node:18.17.1-alpine3.18' }
    }
    stages {
        stage('Test') {
            steps {
                bat 'node --version'
            }
        }
    }
}
