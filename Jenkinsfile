pipeline {
  agent any
  environment {
    KUBECONFIG = '/var/lib/jenkins/admin.conf'
      }
  stages {
        stage('Convert Script to Unix Format') {
            steps {
                script {
                    // Convert the script to Unix format
                    sh 'dos2unix get-k8s-info.sh'
                }
            }
        }

        stage('Run get-k8s-info Script') {
            steps {
                script {
                    // Run the script with parameters and automatically answer "y" to prompts
                    sh 'yes | ./get-k8s-info.sh --case CS0000000 --namespace sit --logs sas.com/deployment=sas-viya --deploypath /var/lib/jenkins/viya_sit --out /root/getinfo'
                }
            }
        }
    }
}
