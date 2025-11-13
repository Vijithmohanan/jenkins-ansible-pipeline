pipeline {
  agent any

  stages {
    stage('Run Ansible on EC2') {
      steps {
        sh '''
          ssh -i ~/.ssh/id_rsa ec2-user@98.88.29.50 \
          'ansible-playbook /home/ec2-user/playbook.yml'
        '''
      }
    }
  }
}

