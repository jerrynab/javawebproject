pipeline {
    agent any
        parameters {
            string(defaultValue: "", description: 'VM name', name: 'VM_Name')
        }
  stages {
        stage('Copy Artifact') {
            steps {
                script {
                        copyArtifacts filter: 'my-file.txt', projectName: 'Project-A-Job', selector: lastSuccessful(), target: workspace
                }
            }
        }
       }
}
