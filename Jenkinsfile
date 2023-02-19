pipeline{
    agent any
    stages{
        stage('Build'){
            steps{
                sh 'g++ -c main/PES1UG20CS508.cpp'
                sh 'g++ -o PES1UG20CS508 main/PES1UG20CS508.cpp'
                echo 'build stage successfull'
            }
        }
        stage('Test'){
            steps{
                sh './PES1UG20CS508'
                echo 'test stage successful'
            }
        }
        stage('Deploy'){
            steps{
          
                echo 'Deployment Successful'
            }
        }
    }
    post{
        failure{
            echo 'Pipeline Failed'
        }
    }
}