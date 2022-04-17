properties([pipelineTriggers([pollSCM('H/20 * * * *')])])
pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git "https://github.com/ikutielmayer/MySoftware.git"
            }
        }
         stage('Build') {
            steps {
                sh "python3 NewButton.py"
            }
        }
    }
}
