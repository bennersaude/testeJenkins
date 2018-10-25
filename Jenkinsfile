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
            steps {                
                echo "TESTE"
            }
        }
        stage('Stage2') {
            steps {                
                echo "TESTE"
            }
        }
    }
}

