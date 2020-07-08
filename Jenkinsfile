node{
  echo "CSC_LINK:${env.CSC_LINK}"
  echo "GH_TOKEN:${env.GH_TOKEN}"
  checkout scm
  bat 'npm install'
  bat 'npm run build-windows'
 
  }
