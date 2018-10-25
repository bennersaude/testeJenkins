pipeline {
   agent any
    stages {
        stage('Stage1') {
            steps {                
				script {
                    def caminho = ${WORKSPACE}
                    println caminho
                }
            }
        }
        stage('Stage2') {
            steps {                
                echo ${WORKSPACE}
            }
        }
    }
}

