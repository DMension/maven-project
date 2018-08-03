pipeline {
    agent any
    stages{
        stage('Build'){
            steps {
                //sh 'mvn clean package'
                echo 'this is the first step...'
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