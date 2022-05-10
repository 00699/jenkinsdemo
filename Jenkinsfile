node(){
    try {
        stage("Checkout Code") {
            println "Checkout stage"
            git url: "https://github.com/00699/cicddemo.git", branch: "main", credentialsId:'sshcreds'
        }
        stage("Build") {
            println "Build stage"
            bat "dir"
        }
        stage("Testing") {
            println "Testing stage"
        }
        stage("Deploy") {
            println "Deploy app"
        }
    } catch(Exception e) {
        println "Exception occured"
    } finally {
        deleteDir()
    }
}
