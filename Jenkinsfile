pipeline {
  agent any
  environment {
    KUBECONFIG = '/var/lib/jenkins/admin.conf'
      }
  stages {
    stage('WP') {
      steps {
        sh 'chmod +x get-k8s-info.sh'
        sh 'get-k8s-info.sh'
      }
    }
  }
}
