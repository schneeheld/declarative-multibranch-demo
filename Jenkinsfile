pipeline {
    agent any
    
    
//    def job="${env.JOB_NAME}" 
//    def jobName= job.substring(job.lastIndexOf("/") + 1, job.length())
//    ws("ws/"+jobName){
    customWorkspace "MyFixedLocation/MyPipelineName_${BRANCH_NAME}"
    stages {
        stage('DeclarativeMultiBranch') {
            steps {
                echo 'Master branch'
                
                script {
                    def students = ['Anne', 'Emily', 'Julie']
                    for (int i = 0; i < students.size(); ++i) {
                        echo "Listing the students: ${students[i]}"
                    }
                }
            }
        }
    }
  //  }
}
