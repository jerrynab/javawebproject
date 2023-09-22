pipeline {
    agent any
parameters {
    string(name: 'ACTIVITY_ID', defaultValue: "1234!")}
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


