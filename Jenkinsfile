node{
  stage('scm checkout'){
    git 'https://github.com/uday-create/pipelineu'
  }
  stage('compile package'){
    def mvnHome = tool name: 'maven-3.6.3', type: 'maven'
    sh "${mvnHome}/bin/mvn package" 
  }
}
  
