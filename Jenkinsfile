pipeline {
    agent any 
    stages {
        stage('Stage 1') {
            steps {
                echo 'Hello world!Main2'
                withCredentials([[ $class: 'AmazonWebServicesCredentialsBinding', credentialsId: 'aws-key', accessKeyVariable: 'AKIA6ODU4FFL7NUXDQUU', secretKeyVariable: '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']]) {
                    echo 'hi fred3'
                    sh 'aws configur --profile fredmac99'
                    sh 'aws s3 ls'
                }
            }
        }
    }
}
