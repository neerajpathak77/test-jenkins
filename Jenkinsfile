


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

         



        steps {

          script {
              name = "SSSSSSS"
           }

          echo "I am inside steps $name"

        }
    }


  }
}

