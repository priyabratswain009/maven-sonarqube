node() {

  stage ('Checkout')
  {
    cleanWs();
  git credentialsId: 'Jenkin-git_inte', url: 'https://github.com/Kamthekirtee/maven-sonarqube.git'
  }
 
  stage ('Build')
  {
  sh 'mvn clean package'
  }

}
