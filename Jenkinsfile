pipeline {
    agent any
        parameters {
            string(defaultValue: "", description: 'VM name', name: 'VM_Name')
        }
    stages {
        stage('PrintParameter'){
            steps{
                 echo "This ansible is running on ${VM_Name}"
            }
        }
    }
}
