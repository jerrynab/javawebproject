pipeline {
    agent any
        parameters {
            string(defaultValue: "", description: 'VM name', name: 'VM_Name')
        }
  stages {
        stage('Write VM_Name to File') {
            steps {
                sh 'echo "${params.VM_Name}" > vm-name.txt'
                stash includes: 'vm-name.txt', name: 'vm-name-stash'
            }
        }
       }
}
