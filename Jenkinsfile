pipeline{
    agent any
    stages {
        stage ('Build'){
            steps {
                echo "Build"
            }
        }
        stage ('Test'){
            steps {
                echo "Test"
            }
        }
        stage ('Integrated Test'){
            steps {
                echo "Integrated Test"
            }
        }
    }
    post{
        success{
            echo "I'm successfull"
            }
        failure{
            echo "I failed"
            }
        }
}