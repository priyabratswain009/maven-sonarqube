node() {

  tool name: 'maven', type: 'maven'
  
  stage ('Checkout')
  {
    cleanWs();
  git credentialsId: 'Kirtee-github-private-key', url: 'https://github.com/Kamthekirtee/maven-sonarqube.git'
  }
 
  stage ('Build')
  {
    withSonarQubeEnv(installationName: 'sonar'){
            sh 'mvn clean package' 
           }
  }

}
