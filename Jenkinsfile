pipeline {
    agent any
    stages {
        stage('DeclarativeMultiBranch') {
            steps {
               echo 'Master branch'
               job="${env.JOB_NAME}" 
               jobName= job.substring(job.lastIndexOf("/") + 1, job.length())
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
