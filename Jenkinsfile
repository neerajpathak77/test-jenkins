


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
              def val = functionInPipeline("NO NAME")
              echo "$val"
              echo "++++++++++++++++env++++++++++++++++++"
              echo "$env.BRANCH_NAME"
              echo "++++++++++++++++env++++++++++++++++++"
           }
        }
    }

  // stage('Trigger other parameterised job from here and pass parameter multi JOB pipeline'){
  //       steps {
  //             build job: 'parameterised_job_called_from_a_jenkinsfile-1', parameters: [string(name: 'testVarible', value: '"Hello I am from varible value passed to me"')]
  //       }
  //     }
  // }
}







