pipeline {
    agent { label 'LinuxAgent1' }

    stages {
        stage('Git') {
            steps {
                echo 'Hello World'
                git credentialsId: 'personal-github-account', url: 'https://github.com/rajaramthumati/java-project.git'
            }
        }
        stage('Hello') {
            steps {
                echo 'Hello World'
            }
        }
    }
}
