pipeline {
    agent any
    tools {
	  maven 'Maven3'
	  jdk 'jdk-17'
	}
	
    stages {
	
  stage('Initialize') {
    steps {
      echo 'Maven version..'
	  bat "mvn -version"
    }
  }
  
  stage('Build') {
      steps {

        bat 'mvn clean install'

      }
  }
	    
  stage('test') {
    steps {
      echo 'Testing....'
    }
  }

  stage('deploy') {
    steps {
      echo 'Deploying...'
      deploy adapters: [tomcat9(credentialsId: 'c4c9ce6d-1e47-4f4d-b99c-4d1c85e297d5', path: '', url: 'http://localhost:8090/')], contextPath: 'webapp', war: '**/*.war'	    
      echo 'Done!'
    }
  }

}

}
