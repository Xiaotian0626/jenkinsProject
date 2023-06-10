pipeline {
    agent {
        node {
            label "docker-agent-alpine"
        }
    }
    

    triggers {
        pollSCM "* * * * *"
    }

    stages {
        stage("build") {
            steps {
                echo "build"
                sh '''
                 echo "doing build stuff..."
                '''
            }
        }

        stage("test") {
            steps {
                echo "test"
                sh '''
                echo "doing test stuff..."
                 '''
            }
        }

        stage("delivery") {
             steps {
                echo "delivery"
                sh '''
                echo "doing delivery stuff..."
                 '''
            }
        }
    }
}
