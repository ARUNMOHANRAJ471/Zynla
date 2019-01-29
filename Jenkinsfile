
node {
  stage: 'Environment Variables'
  sh "env"

  stage 'Checkout Repository'
  git url: 'https://github.com/ARUNMOHANRAJ471/Zynla.git', branch: "master"

  stage 'Installing Dependencies'
  sh "npm prune"
  sh "npm install"

  stage 'Linting'
  sh "npm run gbuild"


  stage 'Testing'
  sh "npm run test"


}

