pipeline {
    agent any
    stages {
        stage('Ok') {
            steps {
                echo "Ok"
            }
        }
    }
    post {
        always {
            emailext body: 'A Test EMail', to: 'shams.watha@gmail.com', subject: 'Test'
        }
    }
}
