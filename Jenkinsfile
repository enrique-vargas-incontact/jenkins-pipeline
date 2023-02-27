pipeline {
    agent any

    stages {
	
 
  stage('Build') {
    steps {
	  try {
        echo 'Building..'
	    bat "javac HelloWorld/HelloWorld.java"
	    bat "cd HelloWorld"
	    bat "java HelloWorld"
	  } catch (err) {
	    echo "Caught: ${err}"
	  }
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
