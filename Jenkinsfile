pipeline {
    agent any

    environment {
            // ENV_URL = "pipeline.global.com"  //declaring at pipeline will allow all stages to access this cvariable
            SSH_CRED = credentials('SSH_CRED')
        }
    stages {
        stage('perform Dry Run') {    
             steps {
                sh "env"
                // sh "ansible-playbook -e ansible_user=${SSH_CRED_USR} -e ansible_password=${SSH_CRED_PSW} -e COMPONENT=Mongodb -e ENV=dev robot-dryrun.yml"
            }

        }

    }
}
//testing on different branch