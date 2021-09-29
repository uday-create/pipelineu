node{
  stage('scm checkout'){
    git 'https://github.com/uday-create/pipelineu'
  }
  stage('compile package'){
    sh 'mvn package'
  }
}
  
