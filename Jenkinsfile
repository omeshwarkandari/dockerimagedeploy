pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade petclinic-app petclinic  --set image.repository=registry.hub.docker.com/omeshwar/petclinic --set image.tag=13'
              			
            }           
        }
    }
}
