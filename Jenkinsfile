pipeline {
    agent { label 'dec' }
        environment {
job="${env.JOB_NAME}.${env.BRANCH_NAME}"
jobName= job.substring(job.lastIndexOf("/") + 1, job.length())
    }
    stages {
        stage('DeclarativeMultiBranch') {
            steps {
               timeout(time: 3, unit: "HOURS") {
                    input message: 'Do you approve install', ok: 'Yes'
               }
               echo 'Master branch'

                    script {
                        def names = ['Anne', 'Emily', 'Julie']
                        for (int i = 0; i < names.size(); ++i) {
                            echo "${names[i]}"
                        }
                    }
            }
        }
    }
}
