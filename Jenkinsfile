pipeline {
    agent any {
        tools {
            jdk 'jdk11'
            npm 'npm6'
        }
        environmentVariables{
            sonarqube 'sonar-token'
        }
        stages{
            stage( 'clean workspae'){
                steps {
                cleanWs
                } 
            }                      
        }
        stage ('Checkout from git'){
            steps {
                with git
            }
        }
        stage (' sonarqube Analysis') {
            steps {
                with
            }
        }
        stage ('Quality Gates') {
            steps{
                withssona
            }
        }
    }
}