pipeline {
    agent any

    

    stages {
        stage('Child Pipeline') {
            steps {
                script {
                    // Use the 'ACTIVITY_ID' parameter passed from the parent
                    def ACTIVITY_ID = params.ACTIVITY_ID
                    echo "Received ACTIVITY_ID from parent: ${ACTIVITY_ID}"
                    // Do other tasks as needed
                }
            }
        }
    }
}

