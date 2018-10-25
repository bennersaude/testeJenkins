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
                echo "Builde14: ${WORKSPACE} "
				ECHO "Nuget: %MSBuild14% "
				ECHO "Nuget: %Orquestrador% "

            }
        }
    }
}

