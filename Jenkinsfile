pipeline{
    agent any

    stages {
        stage("save code") {
            steps{
                script {
                    copy(file:"index.tml", tofile:"output.txt")
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