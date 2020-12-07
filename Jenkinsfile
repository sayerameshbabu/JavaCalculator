pipeline{
  agent any
  environment{
    GITHUB=credentials('git')
  }
  stages{
    stage("test.."){
      steps{
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
