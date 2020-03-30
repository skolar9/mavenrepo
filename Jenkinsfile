pipeline {
    agent any

    stages {
        stage("Build master") {
            when{
                tag "2.0"
            }
            steps{
                echo 'Hello world'
            }
        }
    }
}
