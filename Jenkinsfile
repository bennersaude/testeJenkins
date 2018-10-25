pipeline {
   agent any
   
    stages {
        stage('Stage1') {
            steps {                
				script {
                    def caminho = ${WORKSPACE}
                    println caminho
					println ${sha1}
                }
            }
        }
        stage('Stage2') {
            steps {                
                echo "TESTE"
            }
        }
    }
}

