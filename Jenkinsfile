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
        always {
            currentbuild.result
        }
    }
}

