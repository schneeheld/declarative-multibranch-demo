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
                    script {
                        def names = ['Anne', 'Emily', 'Julie']
                        for (int i = 0; i < names.size(); ++i) {
                            echo "${names[i]}"
                        }
                    }
                sh 'printenv'
                echo "test ${env.CHANGE_AUTHOR_DISPLAY_NAME} --- ${env.BUILD_USER_ID}"
                echo "${env.CHANGE_ID}"
               }
          }
    }
}
