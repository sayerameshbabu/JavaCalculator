pipeline{
  agent any
  environment{
    GITHUB=credentials('git')
  }
  stages{
    stage("test.."){
      steps{
        withCredentials([
          usernamePassword(credentials:'docker', usernameVariable: USER), passwordVariable: PWD1
        ]){
          echo "${PWD1}"
        }
//        echo "${GITHUB}"
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
