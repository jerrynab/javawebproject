pipeline {
    agent any
parameters {
    string(name: 'ACTIVITY_ID', defaultValue: "1234!")}
    stages {
        stage('Child Pipeline') {
            steps {
                script {
                    // Access the environment variable set by the parent pipeline
                    def activityID = env.ACTIVITY_ID
                    echo "Received activityID from parent: ${activityID}"
                    // Do other tasks as needed
                }
            }
        }
        stage('PrintCauses'){
            steps{
                script {
                    def causes = currentBuild.getBuildCauses()
                    println causes
                    def build_id = causes?.upstreamBuild[0] 
                    println build_id
                    def upstream = currentBuild.rawBuild.getCause(hudson.model.Cause$UpstreamCause)
                  echo upstream?.shortDescription
                }
            }
        }
        
    }
}


