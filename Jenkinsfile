pipeline {
    agent any 
    parameters {
        string(defaultValue: "123", description: 'This is a VM name', name: 'VM_Name')
    }
    stages {
        stage('Stash VM_Name') {
            steps {
                stash includes: 'vm-name.txt', name: 'vm-name-stash'
            }
        }
        stage('Trigger Second Jenkinsfile') {
            steps {
                build job: "../javawebproject/master", wait: true;
            }
        }
    }
}
