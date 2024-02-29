pipeline {
    agent any

    parameters {
        choice(name: 'GIT_BRANCH', choices: ['main', 'test1'], description: 'Select the git branch')
    }

    stages {
        stage('Checkout') {
            steps {
                script {
                    // Use the GIT_BRANCH parameter value to determine the branch to checkout
                    checkout([$class: 'GitSCM', branches: [[name: "${params.GIT_BRANCH}"]], 
                              userRemoteConfigs: [[url: 'https://github.com/your/repository.git']]])
                }
            }
        }
        // Add more stages as needed
    }
}
