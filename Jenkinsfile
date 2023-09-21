pipeline {
    agent any

    stages {
        stage('Child Pipeline') {
            steps {
                script {
                    def stashedActivityID = readFile('activityID.txt').trim()
                    echo "Child Pipeline - Received activityID from parent: ${stashedActivityID}"
                    // Do other tasks as needed
                }
            }
        }
    }
}

