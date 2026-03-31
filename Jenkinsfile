pipeline {
    agent any

    stages {
        stage('Getting Repo files') {
            steps {
                git branch: "main", credentialsId: 'github', url: "https://github.com/MohamedMagdy840/jenkins-helloworld.git"
            }
        }

        stage('Hello World') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Hello Jenkins') {
            steps {
                echo 'Hello Jenkins'
            }
        }
    }
}
