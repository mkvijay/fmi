#!groovy
@Library('my-shared-library') _
pipeline {
    agent any

    stages {
        stage ('Compile Stage') {

            steps {
                echo 'Hello World'
            }
        }
        stage ('Testing Stage') {

            steps {
                echo 'pipeline welcome'
            }
        }
        stage ('Deployment Stage') {
            steps {
                echo 'pipeline is working'
            }
        }
    }
    post {
        success {
            slackSend ( channel: 'work-test', color: '#00FF00', message: "pipeline completed (${env.BUILD_URL})" )
        }
        failure {
            slackSend ( channel: 'work-test', color: '#FF0000', message: "pipeline completed (${env.BUILD_URL})" )
        }
    }
}

