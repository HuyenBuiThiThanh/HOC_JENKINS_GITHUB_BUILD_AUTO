pipeline {
    agent any

    stages {
        stage('Clone') {
            steps {
		echo 'Hello World'
		git branch: 'main', credentialsId: 'HuyenBuiThiThanh', url: 'https://github.com/HuyenBuiThiThanh/appHoidanIT_JenkinsFileSCM.git'
                
                }
        }
    }
}
