pipeline {
  agent any


       
        withEnv([]) {
              echo "qwerty"

}
  stages {
    stage ('Compile and Stage') {

          steps {
              sh "npm install"
              sh "npm run build"
          }
    }
  }
}

