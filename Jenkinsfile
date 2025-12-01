pipeline{
    agent any

    stages{
        stage("save changes to file"){
            steps{
        sh "echo index.html > output.txt"
            }
            
    }

    post{
        always{
            archiveArtifacts artifacts: "output.txt"
        }
    }
            


}
