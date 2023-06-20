pipeline {
    agent any 
    triggers {
       upstream 'project-1'
    }
    
    stages {
        stage("Code Checkout") {
            steps {
                git credentialsId: 'ForGitHub', url: 'https://github.com/sekhar-1995/insure-me-selenium.git'
            }
        }
        
         stage("Running the Test-Case") {
            steps {
                sh 'sudo java -jar subham-insure-me.jar'
            }
        }
    }
}
