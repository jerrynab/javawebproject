def upstream_project_build_number(){
    causes = currentBuild.getBuildCauses()
    if (causes?.upstreamBuild[0]){
        build_id = causes?.upstreamBuild[0]
    }
    else{
        build_id = "Root"
    }
    return build_id
}
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
                    def upstream_build_id = upstream_project_build_number()
                    print upstream_build_id
                    print currentBuild.upstreamBuilds[0].projectName

                }
            }
        }
        
    }
}


