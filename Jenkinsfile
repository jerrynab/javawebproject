@Library('globalvarhelper') _
import org.mycompany.SharedVariables

pipeline {
    agent any

    stages {
        stage('Child Pipeline') {
            steps {
                script {
                    def sharedVars = new SharedVariables()
                    echo "Child Pipeline - Received activityID from parent: ${sharedVars.ACTIVITY_ID}"
                    // Do other tasks as needed
                }
            }
        }
    }
}

