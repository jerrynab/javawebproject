pipeline {
    agent any 
 
    stages {
stage('Use activityID in Job') {           
            steps {                  script {
                    // Use the 'ACTIVITY_ID' parameter passed from the parent
                    def activityID = params.ACTIVITY_ID
                    echo "Received activityID from parent: ${activityID}"
                    // Do other tasks as needed      
    }
}
        
    }
}
}


