pipeline {
    agent any
        environment {
job="${env.JOB_NAME}.${env.BRANCH_NAME}"
jobName= job.substring(job.lastIndexOf("/") + 1, job.length())
    }
    stages {
        stage('DeclarativeMultiBranch') {
            steps {
               echo 'Master branch'

               ws('/var/jenkins_home/workspace/'+jobName) {
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
}
