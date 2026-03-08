pipeline {
    agent any

    triggers {
        githubPush()
        cron('H/5 * * * *')
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building project...'
            }
        }

        stage('Test') {
            steps {
                echo 'Running tests...'
            }
        }
    }
}
