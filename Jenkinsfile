pipeline{
    agent any
    stages{
        stage("checkout"){
            steps{
                checkout([$class: 'GitSCM',
                branches: [[name: '*/master']],
                extensions: [],
                userRemoteConfigs: [
                                    [credentialsId: 'saisanthosh23',
                                     url: 'https://github.com/saisanthosh23/webapplication.git']]
                                    ])
            }
        }
        stage("test"){
            steps{
                echo "this is tested"
            }
        }
         stage("QA"){
            steps{
                echo "this is tested"
            }
        }
      stage("build"){
            steps{
                echo "this is tested"
            }
        }  
        stage("artifactory push"){
            steps{
                echo "this is tested"
            }
        }  
        stage("create image"){
            steps{
                echo "this is tested"
            }
        }  
        stage("deploy to k"){
            steps{
                echo "this is tested"
            }
        }  
    }
    post{
        success{
            echo "this is post"
        }
    }
}
