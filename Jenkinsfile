


def name = "none"




pipeline {
  agent any
  stages {
    stage ("Compile and Stage") {

          steps {
              sh "npm install"
              sh "npm run build"
          }
    }
    stage ("Logging") {
        steps {
          name = "I am assigned"
          echo "This stage will be executed first. $name"
        }
    }
  }
}

