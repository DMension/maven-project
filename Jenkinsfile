pipeline {
    agent any
    stages{
        stage('Build'){
            steps {
                echo 'this is the first step...'
                sh 'mvn clean package'
                
            }
            post {
                success {
                    echo 'Now Archiving....'
                    //archiveArtifacts artifacts: '**/target/*.war'
                }
            }
        }
    }
}