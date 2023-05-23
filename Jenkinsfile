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
                git branch: 'main', credentialsId: 'glen-jenkins', url: 'https://github.com/gminezes/Jenkins-Repo.git'
                mkdir 'Git' {
                cp ../Jenkins-Repo/jenkins_home/workspace/Jenkins-Github/Glen2
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
