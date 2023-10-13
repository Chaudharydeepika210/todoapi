pipeline{
    agent {
        docker {
            // Use a .NET SDK image with the version you need
            image 'mcr.microsoft.com/dotnet/sdk:7.0'
            args '-v /var/run/docker.sock:/var/run/docker.sock'
        }
    }
    //agent {docker { image 'mcr.microsoft.com/dotnet/sdk:7.0'} }
 //   agent any
    stages {
        stage ('Build'){
            steps {
                sh 'dotnet --version'
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