pipeline {
    agent any
    stages {
        stage('Use activityID in Job') {
            steps {
                script {
                    withEnv(['ACTIVITY_ID=${env.ACTIVITY_ID}']) {
                        echo "Received activityID: ${ACTIVITY_ID}"
                        // Use ACTIVITY_ID in your job as needed
                    }
                }
            }
        }
    }
}

