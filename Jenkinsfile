node{
  
  stage('checkout') {
   checkout scm;
  }
 
  stage('build') {
    bat '''
       yarn install
       yarn build
       yarn run publish $OS
    '''
    }
  }
