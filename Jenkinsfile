pipeline {
  agent any
  environment {
    KUBECONFIG = '/var/lib/jenkins/admin.conf'
      }
  stages {
    stage('WP') {
      steps {
        sh 'kubectl get nodes'
      }
    }
  }
}
