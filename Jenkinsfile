pipeline {
    agent any
        parameters {
            string(defaultValue: "", description: 'VM name', name: 'VM_Name')
        }
  stages {
        stage('Unstash VM_Name') {
            steps {
                unstash 'vm-name-stash'
                script {
                    VM_Name = readFile('vm-name.txt').trim()
                }
            }
        }
       }
}
