node {
  stage('Hello'){
    echo "Hello Worldd!"
  }
}

pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
                retry(3) {
                    bat 'flakey-deploy'
                }

                timeout(time: 3, unit: 'MINUTES') {
                    bat 'health-check'
                }
            }
        }
    }
}
