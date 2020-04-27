pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        
        stage('Build') {
            steps {
                echo 'Building'
            }
        }
        
        stage('Test') {
            steps {
                echo 'Testing'
            }
        }
        
        stage('Sanity check') {
            steps {
                input "Testing looks ok and ready to deploy?"
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying'
            }
        }
    }
}
