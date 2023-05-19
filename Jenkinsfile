pipeline {
    agent any

    stages {
        stage('Checkout the source repo') {
            steps {
                git branch: 'main', credentialsId: 'sourcecode-bitbucket', url: 'https://github.com/gminezes/git-demo.git'
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}