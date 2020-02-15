


def workspace = 'workspace-none'




pipeline {
  agent any
  stages {
    stage ('Compile and Stage') {

          steps {
              sh "npm install"
              sh "npm run build"
          }
    }
    stage ('Logging') {
      workspace = pwd()
      echo 'workspace is -->> ${workspace}'

    }
  }
}

