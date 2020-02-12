pipeline {
  agent any

  stages {
    stage ('Compile and Stage') {
          steps {
              sh "npm install"
              sh "npm run build"
          }
    }
  }
}
