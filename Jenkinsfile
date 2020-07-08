node{
  
  stage('checkout') {
   checkout scm;
  }
 
  stage('pre') {
    //check()
    bat 'rd -r node_modules'
  }
 
  stage('build') {
    bat '''
       yarn install
       yarn build
       yarn run publish $OS
    '''
    }
  }
