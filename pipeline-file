pipeline{
    agent any
    stages {
    stage("Checkout scm")
{
    steps{
          checkout scm
}
}
        stage('submit stack') {
            steps {
                bat "aws cloudformation create-stack --stack-name Vignesh --template-body file://ec2.yaml --region ap-south-1"
            }
        }

    }

}
