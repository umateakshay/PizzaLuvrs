// Powered by Infostretch 

timestamps {

node () {

	stage ('GITUAT - Checkout') {
 	 checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'GitHub', url: 'https://github.com/umateakshay/PizzaLuvrs.git']]]) 
	}
}
}