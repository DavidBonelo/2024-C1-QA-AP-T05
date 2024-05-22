node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    withSonarQubeEnv('sonarJuanJo') {
      sh "./gradlew sonar"
    }
  }
}