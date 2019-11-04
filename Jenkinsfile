pipeline {
    agent any
    environment{
            docker_tag = getDockertag()
}
stages{
        stage('build docker image'){
            steps{
                sh "docker build . -t rudra8/testapp:${docker_tag}"
            }
        }
    }
def get Dockertag(){
       def tag = sh script: 'git rev-parse HEAD',returnStdout: true
       return tag
 }
}
