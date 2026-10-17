pipeline {
    agent any

    stages {
        stage('get the code from github') {
            steps {
                 // Assuming you have your Ansible playbook in a SCM like Git
                checkout scm
            }
        }
		stage('linux command') {
            steps {
                sh 'cat index.html'
            }
        }
		
    }
}
