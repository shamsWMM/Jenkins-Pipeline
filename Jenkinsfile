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
                echo "Ensuring code works as expected"

                echo "Performing integration testing"
                echo "Ensuring application components work together as expected"

                echo "Tool for unit tests: Unity Test Tool"
                echo "Tool for integration tests: Cypress"
            }
        }
        stage("Code Analysis"){
            steps{
                echo "Analysing code"
                echo "Code works as expected!"

                echo "Performing integration testing"
                echo "Application components work together as expected"

                echo "Tool for unit tests: Unity Test Tool"
                echo "Tool for integration tests: Cypress"
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
