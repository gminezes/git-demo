pipeline {
    agent any

    stages {
        stage('Checkout the source repo') {
            steps {
                git branch: 'main', credentialsId: 'sourcecode-bitbucket', url: 'https://github.com/gminezes/git-demo.git'
                echo 'Building..'
            }
        }
        stage('Copying file') {
            steps {
                git branch: 'main', url: 'https://github.com/gminezes/git-demo.git'
                cp 'Glen2'
           }
        }
    }
}
        stage('Checkout the source repo') {
            steps {
                cp ..git branch: 'main', url: 'https://github.com/gminezes/Jenkins-Repo.git'
                echo 'Deploying....'
            }
        }
    }
}
