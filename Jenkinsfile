node{
  stage('scm checkout'){
    git 'https://github.com/uday-create/pipelineu'
  }
  stage('compile package'){
    def mvnHome = tool name: 'maven-3.6.3', type: 'maven'
    sh "${mvnHome}/bin/mvn package" 
  }
  stage('slack notification'){
    slackSend baseUrl: 'https://hooks.slack.com/services/',
      channel: 'jenkins-pipeline-demo', 
      color: 'good', iconEmoji: 'slack', 
      message: 'hello jenkins', 
      tokenCredentialId: 'slack id',
      username: 'uday'
  }
}
  
