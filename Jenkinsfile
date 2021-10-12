pipeline{
    agent {label 'UBUNTU'}
        triggers { pollSCM ('* * * * *') }
        stages{
            stage('clone and compile') {
                steps {
                    git branch 'declartive', 
                    url:'https://github.com/dumrepo/game-of-life.git'
                    sh 'mvn compile'
                    }
            }
        }
}
