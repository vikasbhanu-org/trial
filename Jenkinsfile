def checkout(){
	dir(BUILD_ID){
		checkout scmGit(branches: [[name: '*/test']], extensions: [], userRemoteConfigs: [[credentialsId: 'git-id', url: 'https://github.com/vikasbhanu-org/trial.git']])
}
}
node{
		stage('checkout into github'){
		checkout()
}
		stage('making a file'){
    sh "echo root | sudo touch /home/ec2-user/demo"
}
}
