pipeline {
	agent any
    stages {
        stage('Build on k8 ') {
            steps {           
                        sh 'pwd'
                        sh 'cp -R helm/* .'
		        sh 'ls -ltr'
                        sh 'pwd'
                        sh '/usr/local/bin/helm upgrade --install petclinic-app petclinic  --set image.repository=registory.hub.docker.com/repository/registry-1.docker.io/mnforba/petclinic --set image.tag=1'
              			
            }           
        }
    }
}
