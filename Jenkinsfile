node{
  
  stage('checkout') {
   checkout scm;
  }
 
  stage('pre') {
    //check()
    bat 'rm -rf node_modules build dist bundle'
  }
 
  stage('build') {
    bat '''
       yarn install
       yarn build
       yarn run publish $OS
    '''
    }
  }
