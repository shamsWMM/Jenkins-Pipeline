pipeline{
    agent any
    environment{
        DIRECTORY_PATH="/Users/shams/Documents/Docs/sit753/CD_pipeline_project"
        TESTING_ENVIRONMENT="CD Pipeline Project TE"
        PRODUCTION_ENVIRONMENT="Shams M Mawlood"

    }
    stages{
        stage('Build'){
            steps{
                echo "Fetch source code from $DIRECTORY_PATH."
                echo "Compile the code and generate necessary artefacts."
                echo "Build stage complete!"
            }
            post{
                success{
                    mail to: "shams.alsaegh@gmail.com"
                    subject: "Build Status Email"
                    body: "Build was successful"

                }
                failure{

                }
                always{

                }
            }
        }
        stage('Test'){
            steps{
                echo "Start unit tests."
                echo "Start integration tests."
                echo "Test stage complete!"
            }
        }
        stage('Code Quality Check'){
            steps{
                echo "Check code quality."
                echo "Code quality check stage complete!"
            }
        }
        stage('Deploy'){
            steps{
                echo "Deploy application to $TESTING_ENVIRONMENT testing environment"
                echo "Deploy stage complete!"
            }
        }
        stage('Approval'){
            steps{
                echo "Start approval."
                sleep(time: 10, unit: 'SECONDS')
                echo "Approval stage complete!"
            }
        }
        stage('Deploy to Production'){
            steps{
                echo "Deploy to $PRODUCTION_ENVIRONMENT"
                echo "Deploy to production stage complete!"
            }
        }
    }
}