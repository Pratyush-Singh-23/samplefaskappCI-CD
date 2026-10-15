pipeline {
    agent { label 'worker1' }

    stages { //collection of jobs
        stage ('Run the docker container'){ //job1
        steps{
            sh 'docker rm -f webos'
            sh 'docker pull pratyushsingh23/samplefaskapp'
            sh 'docker run -dit --name webos -p 80:80 pratyushsingh23/samplefaskapp'
        }
        }
    }
}