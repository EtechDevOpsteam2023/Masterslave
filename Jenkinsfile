pipeline{
	agent{
		label 'slave1'
	}
	stages{
		stage('1-clone'){
			steps{
				echo "my first stage"
			}
		}
		stage('2-second slave'){
			agent{
				label 'slave2'
			}
			steps{
				sh 'lscpu'
			}
		}
	}
}