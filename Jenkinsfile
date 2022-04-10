pipeline {
  agent any
  stages 
    {

    stage ('SCM Checkout') {
            steps {
                git branch: 'main', credentialsId: 'bd76dfcf-5cfb-47b3-8292-f684d72ae500', url: 'https://github.com/NightmareNight-em/devops_calculator'
            }
        }

    stage('mvn goals') {
      steps {
        bat 'mvn clean compile test package'
      }
    }
  }
}
