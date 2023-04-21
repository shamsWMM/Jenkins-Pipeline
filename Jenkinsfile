pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                echo "Building..."
            }
            post{
                success{
                    mail to:"shams.watha@gmail.com"
                    subject: "Build Status Email"
                    body: "Build successful!"
                }
            }
        }
    }
}
