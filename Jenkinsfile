pipeline {
    agent any
    parameters {
        string(name: 'ACTIVITY_ID_PARAM', defaultValue: 'ACTIVITY_ID_PLACEHOLDER', description: 'Activity ID from parent pipeline')
    }
    stages {
        stage('Use activityID in Job') {
            steps {
                script {
                    echo "Received activityID: ${params.ACTIVITY_ID_PARAM}"
                    // Use ACTIVITY_ID_PARAM in your job as needed
                }
            }
        }
    }
}



