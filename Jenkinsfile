node() {

  stage ('Checkout')
  {
    cleanWs();
  git credentialsId: 'Kirtee-github-private-key', url: 'https://github.com/Kamthekirtee/maven-sonarqube.git'
  }
 
  stage ('Build')
  {
  sh 'mvn clean package'
  }

}
