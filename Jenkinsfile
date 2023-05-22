pipeline {
    agent any

    stages {
        stage('Checkout the source repo') {
            steps {
                git branch: 'main', credentialsId: 'sourcecode-bitbucket', url: 'https://github.com/gminezes/git-demo.git'
                echo 'Building..'
            }
        }
        stage('commit and push') {
            steps {
                mkdir('Git') {
                cp .."git branch: 'main', url: 'https://github.com/gminezes/git-demo.git" "git branch: 'main', url: 'https://github.com/gminezes/Jenkins-Repo.git"
                    git add 'Glen2'
                    git commit -m "Added new file"
                    git push
                '''
           }
        }
    }
}
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
