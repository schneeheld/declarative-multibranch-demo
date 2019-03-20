pipeline {
    agent any
    stages {
        stage('DeclarativeMultiBranch') {
            steps {
               echo 'Master branch'
               ws('/var/jenkins_home/workspace/zd72694_master-ABCDE') {
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
