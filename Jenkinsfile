pipeline {
  agent any
  tools{
    maven 'MAVEN'
  }
   stages{
    stage('Build'){
      steps{
        echo 'Building Application'
        checkout scmGit(branches: [[name: '*/main']], browser: github('https://github.com/manubolutharunsaireddyms/JavaProject.git'), extensions: [], userRemoteConfigs: [[credentialsId: '3c85ce6c-e4e5-4f8c-b913-4af0dbad5205', url: 'https://github.com/manubolutharunsaireddyms/JavaProject.git']])
      }
    }
  }
}
