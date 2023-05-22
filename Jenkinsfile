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
                cp ..'/var/jenkins_home/workspace/Jenkins-Github/Glen2
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
