pipeline{
    agent any

    stages{

        stage('Build Docker image'){

            steps{
                scrip {
                    dockerapp = docker.build("marcospedrotti/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
                }
            }



        }


    }

}