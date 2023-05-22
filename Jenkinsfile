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
           dir('Git') {
                /**
                 * Copies the downloaded file from repo1 into the 
                 * directory where we cloned repo2 then executing the 
                 * appropriate git commands
                 **/
                bat '''
                    cp ../https://github.com/gminezes/git-demo/blob/main/Glen2.txt .
                    git add Glen2
                    git commit -m "Added new file"
                    git push git branch: 'main', url: 'https://github.com/gminezes/Jenkins-Repo.git'
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
