pipeline{
  agent any
  tools{
    maven 'Maven1'
  }
  
  stages{
    stage("build"){
      steps{
        sh "mvn clean install"
        sh "mvn  clean package"
      }
    }
  }
}
