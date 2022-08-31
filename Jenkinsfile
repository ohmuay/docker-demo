pipeline {
    agent any{
        stages{
            stage("Cloning git"){
                steps {
                    checkout scm
                }                
            }
            stage("Testing client"){
                steps {
                    sh 'echo testing client'
                }
            }
            stage("Testing backend"){
                steps {
                    sh 'echo testing backend'
                }
            }
            stage("Start the server"){
                steps {
                    sh 'docker-compose up --build'
                }
            }
        }
    }
}