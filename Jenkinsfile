pipeline {
    agent any

    stages {
	
 
  stage('Build') {
    steps {
      echo 'Building..'
      bat 'javac HelloWorld/HelloWorld.java'
      bat 'cd HelloWorld'
      bat 'java HelloWorld'
    }
  }

  stage('Deploy') {
    steps {
      echo 'Deploying...'
      echo 'Done!'
    }
  }

}

}
