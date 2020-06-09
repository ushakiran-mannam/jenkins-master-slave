
def dockerPublisherName = "ushakiran20"



def gitBranch

properties([pipelineTriggers([githubPush()])])
pipeline {
    agent {
        node {
            label 'aws_node_two'
        }
    }

    stages {
        


        stage('Build') {
            steps {
                
                    sh "docker-compose -f docker-compose.yaml up -d "

                }
            }
        }

        //    stage('Deploy') {
        //        steps {
        //            script {
        //                if(gitBranch == 'master' || gitBranch == 'dev'){
        //                     sh "docker stack deploy --compose-file docker-compose.yml dockerstack3"
        //                }
        //            }
        //        }
        //    }

      

    }