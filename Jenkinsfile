pipeline {
    agent any

    stages {

        stage('Build') {

            steps {
                echo 'Building an app'
            }
        }

	stage('Test') {

            steps {
                echo 'Testing the app'
            }
        }
	
	stage('Deploy') {

            steps {
                echo 'Deploying the app'
            }
        }
    }
    
    
   post { 
        always { 
           emailext body: 'Test summary', subject: 'Test message', to: 'mukundhan.k@tringapps.com'
        }
    }
}
