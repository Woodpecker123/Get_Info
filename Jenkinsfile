pipeline {
  agent any
  environment {
    KUBECONFIG = '/var/lib/jenkins/admin.conf'
      }
  stages {
    stage('WP') {
      steps {
        sh 'chmod +x get-k8s-info.sh'
        sh './get-k8s-info.sh --case CS0000000 --namespace sit --logs sas.com/deployment=sas-viya  --deploypath /var/lib/jenkins/viya_sit --out /root/getinfo'
      }
    }
  }
}
