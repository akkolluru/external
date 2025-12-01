pipeline{
    agent any

    stages {
        stage("save code") {
            steps{
                echo index.html > output.txt
            }
        }

    }
    post{
        always {
            archiveArtifacts artifacts: 'output.txt' 
        }
    }
}