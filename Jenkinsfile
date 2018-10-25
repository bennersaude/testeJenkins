pipeline {
    agent any
    environment {
		
        caminho = "${WORKSPACE}"
		sha = "${sha1}"
		pr = "${PULL_REQUEST}";
		
	}
    stages {
        stage('Stage1') {
            steps {                
				script {
                    println " Caminho ${caminho}"
					println " Commit ${sha} "
					println " Branch atual: ${env.BRANCH_NAME}"
					println "PullRequest: ${pr}"
                }
            }
        }
        stage('Stage2') {
            steps {                
                echo "Nuget:  " %Nuget%
				echo "WorkSpace:  " %WORKSPACE% 
				echo "Builde14:  " %MSBuild14% 

            }
        }
    }
}

