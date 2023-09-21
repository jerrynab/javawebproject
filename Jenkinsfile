pipeline {
    agent any
    stages {
        stage('Use activityID in Job') {
            steps {
                script {
                    echo "Received activityID: ${env.ACTIVITY_ID}"
                    // Use ACTIVITY_ID in your job as needed
                }
            }
        }
    }
}
