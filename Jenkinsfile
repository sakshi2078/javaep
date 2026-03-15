pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git 'https://github.com/sakshi2078/javaep.git'
            }
        }

        stage('Publish') {
            steps {
                publishHTML([
                    allowmissing: true,
                    alwaysLinktoLastBuild: false,
                    KeepAll: false,
                    reportDir: '.',
                    reportFiles: 'index.html',
                    reportName: 'My HTML Page'
                ])
            }
        }
    }
}
