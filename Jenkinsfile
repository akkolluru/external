pipeline{
    agent any

    stages {
        stage("save code") {
            steps{
                script {
                    sh "cat index.html > output.txt"
                    }
            }
        }

    }
    post{
        always {
            archiveArtifacts artifacts: 'output.txt' 
        }
    }
}