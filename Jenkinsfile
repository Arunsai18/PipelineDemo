node {
	withCredentials([[$class: 'UsernamePasswordMultiBinding', credentialsId: 'MyCred',
                    usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD']]) {
                    
        stage('Initiate'){
        	echo "Jenkinsfile execution started"
        }
                    
        stage ('Clone') {
        	git url: 'https://chandan7128@bitbucket.org/chandan7128/pipelineproject.git'
    	}
    	
    	stage ('Build') {
			sh 'gradle build --info'
    	}       
                    
	}
}
