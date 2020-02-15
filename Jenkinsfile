


def name = "Hello";


def functionInPipeline() {
  def name = "I am from function"
  echo ">>>>>> $name <<<<<<<<"
}

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
        steps {
          script {
              name = "SSSSSSS"
           }
          functionInPipeline()
        }
    }


  }
}

