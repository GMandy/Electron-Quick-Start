node{
  
  checkout scm
  bat 'npm install'
  withEnv(["GH_TOKEN='d389c80262bb997e0b5fa095fc57d86af3a9617d' "]) {
          echo env.GH_TOKEN
          bat 'npm run build-windows'
  }
  
  }
