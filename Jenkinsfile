pipeline {
    agent any
    stages{
        stage('Clone') {
            steps {
                echo 'Clone start'
                git branch: 'main', credentialsId: 'github', url: 'https://github.com/tungk36dl/T3H_Devops2502.git'
                echo 'Clone finish'
            }
        }
   
         stage('Docker') {
            steps {
                echo 'Docker start'
                // This step should not normally be used in your script. Consult the inline help for details.
                withDockerRegistry(credentialsId: 'cred-docker-hub-2', url: '') { // url default https://index.docker.io/v1/
                // some block
                sh label: '', script: 'docker build -t tungpt55/my-web .'
                sh label: '', script: 'docker push tungpt55/my-web'
                echo 'Docker finish'
                }
            }
        }
    }
}