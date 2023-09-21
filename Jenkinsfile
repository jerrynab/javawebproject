pipeline {
    agent any
    environment {
        ACTIVITY_ID = 'ACTIVITY_ID_PLACEHOLDER'
    }
    stages {
        stage('Use activityID in Job') {
            steps {
                echo "Received activityID: ${ACTIVITY_ID}"
                // Use ACTIVITY_ID in your job as needed
            }
        }
    }
}



