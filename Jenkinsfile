pipeline {
    agent any
  
    
  
stages{
        stage('Build'){
            steps {
                sh ' mvn clean package'
            }
            post {
                success {
                    echo 'Now1 Archiving...'
                    archiveArtifacts artifacts: '**/target/*.war'
                }
            }
        }

        
    }
}