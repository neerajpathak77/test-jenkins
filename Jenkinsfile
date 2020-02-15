


def name = "Hello";


def functionInPipeline(aggument) {
  def name = "I am from function"
  echo ">>>>>> $name <<<<<<<<"

  return "aggument passed to me was $aggument"
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
          def val = functionInPipeline("neeraj")
          echo "$val"
        }
    }


  }
}

