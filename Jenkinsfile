pipeline{
    agent any
    stages{
        stage("compile"){
            steps{
                bat 'javac Lion.java'
            }
        }
        stage("run"){
            steps{
                bat"java Lion"
            }
        }
    }
}