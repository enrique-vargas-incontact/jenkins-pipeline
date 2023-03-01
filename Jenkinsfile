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
      echo 'Done!'
    }
  }

}

}
