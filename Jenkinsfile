pipeline{
    // agent {
    //     docker {
    //         // Use a .NET SDK image with the version you need
    //         image 'mcr.microsoft.com/dotnet/sdk:7.0'
    //         args '-v /var/run/docker.sock:/var/run/docker.sock'
    //     }
    // }
    //agent {docker { image 'alpine:3.17'} }
    agent any
    environment{
        dockerHome = tool 'mydocker'
        PATH = "$dockerHome/bin:$PATH"
    }

    stages {
        stage ('Build'){
            steps {
                //sh 'node --version'
                //sh 'docker version'
                echo "Build"
                echo "PATH - $PATH"
                echo "BUILD_NUMBER - $env.BUILD_NUMBER"
                echo "BUILD_ID - $env.BUILD_ID"
                echo "JOB_NAME - $env.JOB_NAME"
                echo "BUILD_TAG - $env.BUILD_TAG"
                echo "BUILD_URL - $env.BUILD_URL"
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