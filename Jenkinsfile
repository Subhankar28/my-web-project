pipeline {
    agent any

    environment {
        GIT_REPO = 'https://github.com/Subhankar28/my-web-project.git'  // Replace with your GitHub repository URL
        BRANCH_NAME = 'main'  // Replace with your branch name if it's different
    }

    stages {
        stage('Clone Code') {
            steps {
                echo 'Cloning the code from GitHub'
                git url: "${GIT_REPO}", branch: "${BRANCH_NAME}"
            }
        }

        stage('Build') {
            steps {
                echo 'Building the project'
                // No build steps for a simple HTML/CSS/JS project
                echo 'Build successful!'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests (if any)'
                // You can add testing scripts here if needed
                echo 'Tests completed!'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Deploying the project'
                // For now, just echo a success message
                echo 'Project deployed successfully!'
            }
        }
    }
}
