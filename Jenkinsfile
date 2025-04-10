pipeline {
    agent any
    stages{
        stage('Clone') {
            steps {
                echo 'Clone code from github'
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