pipeline {
  agent any
  stages {
        stage('WP') {
      steps {
        sh 'kubectl get nodes'
      }

  }
  }
     environment {
    KUBECONFIG = '/var/lib/jenkins/admin.conf'
  }
}
