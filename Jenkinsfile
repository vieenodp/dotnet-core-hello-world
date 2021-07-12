pipeline {
	agent any
	stages {
	stage ('Clean workspace') {
		steps {
			cleanWs()
		}
	}
 
	stage('Checkout') {
		steps {
			checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/vieenodp/dotnet-core-hello-world.git']]])

  }

}
	}
}
