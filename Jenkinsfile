pipeline{
    agent any

    stages{
        stage("save changes to file"){
        echo index.html > output.txt
        archiveArtifacts artifacts: "output.txt"
    }

}
}