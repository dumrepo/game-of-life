pipeline{
    agent {label 'UBUNTU'}
       parameters{string(name: '', defaultValue: '', description: '')}
       parameters { text(name: '', defaultValue: '\n', description: '') }
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

