pipeline {
    agent any
    environment {
		
        caminho = "${WORKSPACE}"
		sha = "${sha1}"
		pr = "${PULL_REQUEST}";
		
		orquestrador = '"${env.Orquestrador}"'
		
	}
    stages {
	
        stage('Stage1') {
            steps {                
				script {
                    println " Caminho ${caminho}"
					println " Commit ${env.sha1} "
					println " Branch atual: ${env.BRANCH_NAME}"
					println "BRANCH_NAME: ${env.BRANCH_NAME}"
					println "CHANGE_ID: ${env.CHANGE_ID}"
					println "CHANGE_URL: ${env.CHANGE_URL}"
					println "CHANGE_TITLE: ${env.CHANGE_TITLE}"
					println "CHANGE_AUTHOR: ${env.CHANGE_AUTHOR}"
					println "CHANGE_AUTHOR_DISPLAY_NAME: ${env.CHANGE_AUTHOR_DISPLAY_NAME}"
					println "CHANGE_AUTHOR_EMAIL: ${env.CHANGE_AUTHOR_EMAIL}"
					println "CHANGE_TARGET: ${env.CHANGE_TARGET}"
					println "BUILD_NUMBER: ${env.BUILD_NUMBER}"
					println "BUILD_ID: ${env.BUILD_ID}"
					println "BUILD_DISPLAY_NAME: ${env.BUILD_DISPLAY_NAME}"
					println "JOB_NAME: ${env.JOB_NAME}"
					println "JOB_BASE_NAME: ${env.JOB_BASE_NAME}"
					println "BUILD_TAG: ${env.BUILD_TAG}"
					println "EXECUTOR_NUMBER: ${env.EXECUTOR_NUMBER}"
					println "NODE_NAME: ${env.NODE_NAME}"
					println "NODE_LABELS: ${env.NODE_LABELS}"
					println "WORKSPACE: ${env.WORKSPACE}"
					println "JENKINS_HOME: ${env.JENKINS_HOME}"
					println "JENKINS_URL: ${env.JENKINS_URL}"
					println "BUILD_URL: ${env.BUILD_URL}"
					println "JOB_URL: ${env.JOB_URL}"		
                }
            }
        }
        stage('Stage2') {
            steps {                
                echo "WorkSpace: ${WORKSPACE} "
				println "MsBuild: ${env.MSBuild14} "
				echo "Orquestrador: ${env.Orquestrador} "
				echo "NUnit3: ${env.NUnit3} "
            }
        }
		stage('Orquestrador') {
			steps{
				bat('%orquestrador% -acao VALIDAR_VERSAO_SMS -repositorio Corrente -pull-request 123')
			}
		}
    }
}
