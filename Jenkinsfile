pipeline{
  agent any
  environment{
    GITHUB=credentials('git')
  }
  stages{
    stage("test.."){
      steps{
        withCredentials([usernamePassword(credentialsId:'docker', usernameVariable:USER, passwordVariable:PASSWORD)]){
          echo "${USER}"
        }
        echo "${GITHUB}"
      }
    }
    stage("build.."){
      steps{
      echo "building"
      }
    }
    stage("deploy.."){
      steps{
      echo "deplying"
      }
    }
  }
}
