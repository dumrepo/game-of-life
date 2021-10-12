pipeline{
    agent {label 'MASTER'}
       parameters { booleanParam(name: 'Buld', defaultValue:false, description: 'This option will be default true') }
	stages{
            stage('clone and compile') {
                steps {
                    git branch: 'declartive', 
                    url:'https://github.com/dumrepo/game-of-life.git'
                    sh 'mvn package'
                    }
            }
        }
}



