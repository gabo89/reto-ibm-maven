pipeline {
   agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		sh './create.sh'
            }
        }     
	stage('publish') {
            steps {
                echo 'starting app....'
		sh './publish.sh'
            }
        }

      	stage('Deliver') {
            steps {
                echo 'starting app....'
		sh './deploy.sh'
            }
        }
    }
}

