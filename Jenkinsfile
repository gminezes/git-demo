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
           dir('repo2') {
                cp ../var/jenkins_home/workspace/Jenkins-Github .
                    git add Glen2
                    git commit -m "Added new file"
                    git push 'branch: 'main', url: 'https://github.com/gminezes/Jenkins-Repo.git'
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
