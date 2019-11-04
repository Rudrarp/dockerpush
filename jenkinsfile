pipeline {
    agent any
    stages{
        stage('build docker image'){
            steps{
                sh "docker build . -t rudra8/testapp:v1"
            }
        }
    }
}
