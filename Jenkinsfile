pipeline {
    agent any 
    parameters {
        string(defaultValue: "123", description: 'This is a VM name', name: 'VM_Name')
    }
    stages {
        stage('Use VM_Name in Job') {           
            steps {                 sh "echo 'Received VM_Name: ${params.VM_Name}'"                 // Use VM_Name in your job as needed                      
    }
}
    }
}
