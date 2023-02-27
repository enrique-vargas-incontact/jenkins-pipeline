pipeline {
    agent any
    tools {
	  maven 'Maven3'
	}
	
    stages {
	
  stage('Load Tools') {
    steps {
      echo 'Loading Tools..'
	  bat "mvn -version"
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
