pipeline {
  agent any
  tools{
    maven 'MAVEN'
  }
   stages{
    stage('Maven Build'){
      steps{
        checkout scmGit(branches: [[name: '*/main']], browser: github(''), extensions: [], userRemoteConfigs: [[credentialsId: '3c85ce6c-e4e5-4f8c-b913-4af0dbad5205', url: 'https://github.com/manubolutharunsaireddyms/JavaProject.git']])
        sh "mvn -Dmaven.test.failure.ignore=true clean package"
      }
    }
  }
}
