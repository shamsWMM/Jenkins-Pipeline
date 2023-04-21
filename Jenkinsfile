pipeline{
    agent any
    stages{
        stage("Build"){
            steps{
                echo "Compiling and packaging the code"
                echo "Tool for build automation: Gradle"
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
                echo "Tool for unit tests: JUnit"
                echo "Tool for integration tests: Cypress"
            }
        }
        stage("Code Analysis"){
            steps{
                echo "Analysing code"
                echo "Code meets industry standards"
                echo "Tool for code analysis: SonarQube"
            }
        }
        stage("Security Scan"){
            steps{
                echo "Scanning code"
                echo "Looking for vulnerabilities"
                echo "Tool for security scanning: OWASP Zed Attack Proxy (ZAP)"
            }
        }
        stage("Deploy to Staging"){
            steps{
                echo "Deploying to staging"
                echo "Staging server: Azure Virtual Machines"
                echo "Use terraform workspaces to switch between spaces"
            }
        }
        stage("Tests on Staging"){
            steps{
                echo "Performing integration testing on staging"
                echo "Ensuring application functions in staging"
                echo "Tool for integration tests: Cypress"
            }
        }
        stage("Deploy to Production"){
            steps{
                echo "Deploying to production"
                echo "Production server: Azure Virtual Machines"
                echo "Use terraform workspaces to switch between spaces"
            }
        }
    }
}
