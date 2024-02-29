pipeline{
    agent any 
        
  environment {

      ArchiveDir = "/home/jenkinbuild"
              repoUrl = "https://github.com/SurenMalkist/jenkins"
		          ProjectName = "Nats"

	    }
      stages {
        stage('Code Checkout'){

			            steps{

			               	step([$class: 'WsCleanup'])

			                		echo "Cloning the ${ProjectName} project from Github"
					                checkout scm
				                	//git credentialsId: 'guru-github-credentials', url: 'https://github.com/netsys-usa/PL_UI.git'
					               echo "Code has been checked out into ${JENKINS_HOME}/workspace/${JOB_NAME} workspace..!"

			            }
        
    



