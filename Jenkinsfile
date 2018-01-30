#!groovy
@Library('my-shared-library') _
pipeline {
    agent any

    stages {
        stage 'Compile Stage' {

            steps {
                echo 'Hello World'
            }
        }
        stage 'Testing Stage' {

            steps {
                echo 'pipeline welcome'
            }
        }
        stage 'Deployment Stage' {
            steps {
                echo 'pipeline is working'
            }
        }
    }
    post {
        always {
            notifier currentBuild.result
        }
    }
}

