pipeline{
    agent any

    stages{
        stage("save changes to file"){
            steps{
        echo index.html > output.txt
        archiveArtifacts artifacts: "output.txt"
            }
    }
            

}
}
