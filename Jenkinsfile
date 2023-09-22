pipeline {
    agent any

    stages {
        stage('Child Pipeline') {
            steps {
                script {
                    // Access the environment variable set by the parent pipeline
                    def activityID = env.ACTIVITY_ID
                    echo "Received activityID from parent: ${activityID}"
                    // Do other tasks as needed
                }
            }
        }
    }
}


