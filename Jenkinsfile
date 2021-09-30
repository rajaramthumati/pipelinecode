pipeline {
    agent { label 'linux1' }
    parameters { string(name: 'branch', defaultValue: 'main', description: '')
                booleanParam(name: 'DEBUG_BUILD', defaultValue: true, description: '')
               }

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
