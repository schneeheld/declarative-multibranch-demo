pipeline {
    agent any
    stages {
        stage('DeclarativeMultiBranch') {
            steps {
                echo 'Hello World'
                script {
                    def students = ['Anne', 'Emily', 'Julie']
                    for (int i = 0; i < students.size(); ++i) {
                        echo "Listing the students: ${students[i]}"
                    }
                }
            }
        }
    }
}
