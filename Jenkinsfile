pipeline {
  agent any
  stages 
    {

    stage ('SCM Checkout') {
            steps {
                git credentialsId: 'github-credentials', url: 'https://github.com/NightmareNight-em/devops_calculator.git'
            }
        }

    stage('mvn goals') {
      steps {
        bat 'mvn clean compile test package'
      }
    }
  }
}
