node{
  stage('scm checkout'){
    git 'https://github.com/uday-create/pipelineu'
  }
  stage('compile package'){
    def mvn-home = tool name: 'maven-3.6.3', type: 'maven'
    def "${mvn-home}/bin/mvn package" 
    sh 'mvn package'
  }
}
  
