pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
		echo 'Hello World'
		git branch: 'main', credentialsId: 'HuyenBuiThiThanh', url: 'https://github.com/HuyenBuiThiThanh/HOC_JENKINS_GITHUB_BUILD_AUTO.git'
                
                }
        }
    }
}
