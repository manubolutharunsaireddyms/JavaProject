pipeline {
  agent any
  tools{
    maven 'MAVEN'
  }
   stages{
    stage('Git Checkout'){
      steps{
        git credentialsId:'github',url:'https://github.com/manubolutharunsaireddyms/JavaProject.git' 
      }
    }
    stage('Maven Build'){
      steps{
        sh "mvn clean package"
      }
    }
  }
}
