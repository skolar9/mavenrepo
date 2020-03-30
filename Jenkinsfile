pipeline {
    agent any

    stages {
        stage("Build master") {
            when{
                buildingTag()
            }
            steps{
                echo 'Hello world'
            }
        }
    }
}
