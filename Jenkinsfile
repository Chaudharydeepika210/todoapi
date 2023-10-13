pipeline{
    agent {docker { image 'mcr.microsoft.com/dotnet/sdk:7.0'} }
 //   agent any
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