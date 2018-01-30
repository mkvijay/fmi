#!groovy
@Library('my-shared-library') _
pipeline {
    node
    stages {
        stage ('Compile Stage') {
             echo 'Hello World'
        }
        stage ('Testing Stage') {
             echo 'pipeline welcome'
            }
        stage ('Deployment Stage') {
             echo 'pipeline is working'
            }
    }
    post {
        always {
            notifier currentBuild.result
        }
    }
}

