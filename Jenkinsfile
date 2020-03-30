pipeline {
    agent any

    stages {
        stage("Build master") {
            when{
                branch 'master'
            }
            steps {
              echo 'building  master'
            }
        }
         stage("Build dev") {
              when{
                branch 'dev'
            }
            steps {
                echo 'building  dev'
            }
        }
    }
}
