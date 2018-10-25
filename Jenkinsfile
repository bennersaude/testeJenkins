pipeline {
   agent {
        node {
            label 'teste'
            customWorkspace '/ts1'
        }
    }

    stages {
        stage('Preparation') {
            steps {                
				script {
                    def caminho = '${WORKSPACE}'
                    println caminho
					println caminho
                }
            }
        }
    }
}

