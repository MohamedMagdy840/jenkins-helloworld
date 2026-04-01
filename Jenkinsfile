pipeline {
    agent any

    parameters {
        choice(
            name: 'ENVIRONMENT', 
            choices: ['dev', 'stg', 'prod'],
            description: 'Select the environment'
        )
    }

    stages {
        stage('Getting Repo files') {
            steps {
                git branch: "main", url: "https://github.com/MohamedMagdy840/jenkins-helloworld.git"
            }
        }

        stage('Hello World') {
            steps {
                echo "Hello World from ${params.ENVIRONMENT}"
            }
        }

        stage('Hello Jenkins') {
            steps {
                echo "Hello Jenkins from ${params.ENVIRONMENT}"
            }
        }
    }
}
