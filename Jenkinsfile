pipeline {
 agent any
 tools {
    maven "maven3"
  }
  stages {
    stage('get scm') {
      steps {
	  git credentialsId: 'github_credentials', url: 'https://github.com/Sahaja1/springapp-seedproject.git'
       }
    }
	stage('mavenbuild'){
	   steps{
	    sh 'mvn package'
	   }
	   }
  }
}

