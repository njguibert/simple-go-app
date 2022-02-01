pipeline {
    agent any
    stages {
        stage('build') {
            steps {
            	retry(3){
            		bat 'go build .\\src\\main.go'
            		bat 'copy main.exe C:\\Appz\\Path'
            	}
            timeout(time: 3, unit: 'MINUTES') {
                    bat 'echo ya aiting 3 minuto'
            	}                        
            }
        }
    }
}