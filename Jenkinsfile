pipeline {
    agent any 
    parameters {
        string(defaultValue: "123", description: 'This is an activityID', name: 'activityID')
    }
    stages {
        stage('Use activityID in Job') {           
            steps {                 sh "echo 'Received activityID: ${params.activityID}'"                 // Use VM_Name in your job as needed                      
    }
}
    }
}
