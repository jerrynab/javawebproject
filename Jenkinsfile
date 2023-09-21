pipeline {
    agent any 

    stages {
        stage('Example') {             steps {                 script {                     // Set the global environment variable                   
            env.activityID = 'my-value1'                   
            echo "Set activityID to ${env.activityID}"                 }           
                                             }
                         }
        stage('Use activityID in Job') {           
            steps {                 sh "echo 'Received activityID: ${env.activityID}'"                 // Use VM_Name in your job as needed                      
    }
}
    }
}



