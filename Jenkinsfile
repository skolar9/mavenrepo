pipeline {
   agent any

 

   stages {
      stage('Clone') {
          steps{
            sh "rm -rf mavenrepo"
            sh "git clone https://github.com/skolar9/mavenrepo.git"
            sh "mvn clean -f mavenrepo"
          }
      }
      stage("Test"){
          steps{
              sh "mvn test -f mavenrepo"
          }
      }
        stage("Deploy"){
          steps{
              sh "mvn package -f mavenrepo"
          }
      }
   }
}
