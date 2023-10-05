pipeline {
    agent any

    stages {
        stage('Child Pipeline') {
            steps {
                script {
                    // Access the environment variable set by the parent pipeline
                    
                    echo "Received activityID from parent: ${params.ACTIVITY_ID}"
                    // Do other tasks as needed
                }
            }
        }

    }
}

