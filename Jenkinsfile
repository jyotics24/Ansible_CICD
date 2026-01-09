pipeline {
    agent any  // Run this pipeline on any available agent

    stages {
        // Stage to deploy NGINX web server using Ansible
        stage('Deploy NGINX') {
            steps {
                // Execute the Ansible playbook for NGINX deployment
                sh 'ansible-playbook -i inventory deploy-nginx.yml'
            }
        }

        // Stage to deploy MySQL database using Ansible
        stage('Deploy MySQL') {
            steps {
                // Execute the Ansible playbook for MySQL deployment
                sh 'ansible-playbook -i inventory deploy-mysql.yml'
            }
        }
    }
}