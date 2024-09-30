pipeline {
  agent any
  environment {
    KUBECONFIG = '/var/lib/jenkins/admin.conf'
      }
     stages {
        stage('Run get-k8s-info Script') {
            steps {
                script {
                    // Create the output directory and set permissions
                    sh 'mkdir -p /var/lib/jenkins/getinfo'
                    sh 'chmod +x /var/lib/jenkins/getinfo'

                    //sh 'dos2unix get-k8s-info.sh'
                    // Convert the script to Unix format

                    // Run the script with parameters and automatically answer "y" to prompts
                    //sh 'yes | ./get-k8s-info.sh --case CS0000000 --namespace sit --logs sas.com/deployment=sas-viya --deploypath /var/lib/jenkins/viya_sit --out /var/lib/jenkins/getinfo'
                }
            }
        }
    }
}

}
