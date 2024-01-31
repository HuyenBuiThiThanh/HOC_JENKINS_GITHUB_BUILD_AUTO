pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
		echo 'Hello World'
		git branch: 'main', credentialsId: 'HuyenBuiThiThanh', url:'https://github.com/HuyenBuiThiThanh/HOC_JENKINS_GITHUB_BUILD_AUTO.git'
                
                }
        }

		
stage('Build') {
    steps {
        // This step should not normally be used in your script. Consult the inline help for details.
        withDockerRegistry(credentialsId: 'docker-hub', url: 'https://index.docker.io/v1/') {
            script {
                // Thay thế lệnh nohup bằng start /B
                bat 'docker build -t huyenmy44/hoc_jenkins_github_buil_auto:version1 .'
                bat 'docker push huyenmy44/hoc_jenkins_github_buil_auto:version1'
            }
        }
    }
}



    }
}



