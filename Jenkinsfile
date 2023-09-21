pipeline {
    agent any

    stages {
        stage('Child Pipeline') {
            steps {
                script {
                    // Access the shared variable set by the parent pipeline
                    def activityID = currentBuild.sharedVars.ACTIVITY_ID
                    echo "Child Pipeline - Received activityID from parent: ${activityID}"
                    // Do other tasks as needed
                }
            }
        }
    }
}
