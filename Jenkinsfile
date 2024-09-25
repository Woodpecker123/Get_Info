pipeline {
  agent any
  stages {
    stage('checkversion') {
      steps {
          sh 'python3 --version'
          sh 'pip install sasctl'
      }
    }
     stage('run python') {
      steps {
       
        sh 'python3 ModelPublish.py'
      }
    }

  }
}
