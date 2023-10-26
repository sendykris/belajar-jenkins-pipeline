pipeline {
    agent {
        node {
            label "linux && java11"
        }
    }
    stages {
        stage("Build") {
            steps{
                echo("Hellow Build")
            }
        }

        stage("Test") {
            steps{
                echo("Hellow Test")
            }
        }

        stage("Deploy") {
            steps{
                echo("Hellow Deploy")
            }
        }
    }


    post {
        always {
            echo "I will always say Hello again!"
        }
        success {
            echo "Yay, success"
        }
        failure {
            echo "Oh no, failure"
        }
        cleanup {
            echo "Don't care success or error"
        }
    }
}