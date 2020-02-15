


def name = "Hello";




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

         script {
              name = "SSSSSSS"
           }



        steps {

          echo "I am inside steps $name"

        }
    }


  }
}

