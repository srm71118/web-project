pipeline {
    agent any
	environment { 
        LINUX = 'redhat'
    }

    stages {
        stage('Hello') {
            steps {
                echo 'Hello World'
				echo "calling pipeline level variable value is $LINUX"
            }
        }
		stage('linux command') {
            steps {
                sh 'date'
            }
        }
		stage('print varible') {
		environment { 
        CUSTOM = 'jenkins'
    }
			steps {
                sh 'cal'
				echo "calling stage level variable value is $CUSTOM"
            }
        }
    }
}
