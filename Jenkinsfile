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
        post{
            successfull{
                echo "I'm successfull"
            }
            fail{
                echo "I failed"
            }
        }
    }
}