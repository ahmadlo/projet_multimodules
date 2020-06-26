pipeline {
   agent any

   
   stages {
      stage('Build') {
         steps {
            // Get some code from a GitHub repository
            git 'https://github.com/ahmadlo/projet_multimodules.git'
 withMaven(maven: 'maven') {
            // Run Maven on a Unix agent.
            sh "mvn clean package"
 }

            // To run Maven on a Windows agent, use
            // bat "mvn -Dmaven.test.failure.ignore=true clean package"
         }

         
         }
      }
   }

