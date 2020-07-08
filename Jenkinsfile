node{
  bat'set %CSC_LINK%=https://www.dropbox.com/s/path/to/file.p12?dl=1'
  echo "GH_TOKEN:${env.GH_TOKEN}"
  checkout scm
  bat 'npm install'
  bat 'npm run build-windows'
 
  }
