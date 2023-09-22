pipeline {
    agent any

    parameters {
        string(name: 'ACTIVITY_ID', description: 'Activity ID from Parent')
    }

    stages {
        stage('Child Pipeline') {
            steps {
                script {
                    // Use the 'ACTIVITY_ID' parameter passed from the parent
                    def activityID = params.ACTIVITY_ID
                    echo "Received activityID from parent: ${activityID}"
                    // Do other tasks as needed
                }
            }
        }
    }
}

