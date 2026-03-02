pipeline {
    agent any

    stages {
        stage('Fetch') {
            steps {
                echo 'Fetching from repo.....'
                git "https://github.com/sakshi2078/javaep.git"
            }
        }
        stage('Build') {
            steps {
                echo 'Build the program'
                bat "javac hello.java"
            }
        }
        stage('Execute') {
            steps {
                echo 'Executing.....'
                bat "java hello"
            }
        }
    }
    post{
        success{
                echo "Pipeline built successfully"
        }    
        failure{
                echo "Pipeline failed"
        } 
    }
}
