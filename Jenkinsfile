pipeline {
    agent any
    stages {
        stage('Deploy') {
            steps {
		    sh "export AWS_DEFAULT_REGION=us-east-1"
                    sh "aws cloudformation create-stack --stack-name CreateEC2Stack --template-body file://CreateSimpleEC2.json --region 'us-east-1'"                   
            }
        }
    }
}
