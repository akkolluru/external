pipeline{
    agent any

    stages {
        stage("save code") {
            steps{
                script {
                    copy 'index.html', 'output.txt'
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