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
         stage('Build') {
            steps {
                echo 'Build code'
            }
        }
         stage('Test') {
            steps {
                echo 'Run unittest'
            }
        }
         stage('Docker') {
            steps {
                echo 'build image'
                echo 'tag'
                echo 'Pust docker hub'
                echo 'finish'
                echo 'finish 2'
            }
        }
    }
}