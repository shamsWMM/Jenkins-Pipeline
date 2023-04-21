pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                echo "Compiling and packing the code"
                echo "Tool for build automation: Jenkins"
            }
            post{
                always{
                    mail to: "shams.watha@gmail.com",
                    subject: "Build Status Email",
                    body: "Build log attached!"
                }
            }
        }
        stage("Test"){
            steps{
                echo "Performing unit testing"
                echo "Performing integration testing"
            }
        }
        stage("Deploy"){
            steps{
                echo "Deploying ..."
            }
        }
        stage("Complete"){
            steps{
                echo "Completed."
            }
        }
    }
}
