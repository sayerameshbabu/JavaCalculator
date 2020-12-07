pipeline{
  agent any
  
  stages{
    stage("test.."){
      steps{
        def GITHUB=credentials('git')
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
