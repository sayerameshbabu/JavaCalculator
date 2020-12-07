def GV
pipeline{
  agent any
  stages{
    stage('init'){
      steps{
        echo "enter init stage commands"
        script{
         GV=load "script1.groovy"
        }
      }
    }
    stage("build"){
      steps{
        script{
          GV.buildApp()
        }
        echo "building.."
      }
    }
  }
}
