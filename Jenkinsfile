@Library('github.com/releaseworks/jenkinslib') _

node {
  stage("List S3 buckets") {
    withCredentials([[ $class: 'AmazonWebServicesCredentialsBinding', credentialsId: 'aws-key', accessKeyVariable: 'AKIA6ODU4FFL7NUXDQUU', secretKeyVariable: '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']]) {
        AWS("--region=us-east-1 s3 ls")
    }
  }
}
