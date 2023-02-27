pipeline {
    agent any

    stages {
	
  stage('Source') {
    steps {
      echo 'Checking out..'
	  checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'github-private-key', url: 'git@github.com:enrique-vargas-incontact/jenkins-pipeline.git']])
    }
  }
  
  stage('Build') {
    steps {
      echo 'Building..'
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
