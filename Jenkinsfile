pipeline{
    agent any
    stages{
        stage("compile"){
            steps{
                sh 'javac Lion.java'
            }
        }
        stage("run"){
            steps{
                sh "java Lion"
            }
        }
    }
}