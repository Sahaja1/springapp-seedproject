pipeline {
 agent any
  stages {
    stage('get scm') {
      steps {
	  git credentialsId: 'github_credentials', url: 'https://github.com/Sahaja1/spring3-mvc-maven-xml-hello-world.git'
       }
    }
	stage('mavenbuild'){
	   steps{
	    sh 'mvn package'
	   }
	   }
  }
}

