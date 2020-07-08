node{
  checkout scm;
  //def noCacheToBuild = load("${WORKSPACE}/.jenkins/noCacheToBuild.groovy")
  def check = load("${WORKSPACE}/.jenkins/check.groovy")
 
  stage('pre') {
    check()
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
