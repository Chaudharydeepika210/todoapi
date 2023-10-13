pipeline{
 //   agent any
    agent { docker { image 'maven: 3.6.3'} }
    stages {
        stage ('Build'){
            steps {
                sh 'mvn --version'
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