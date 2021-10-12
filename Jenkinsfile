pipeline{
    agent {label: 'UBUNTU'}
        trigger{ pollscm('* * * * *') }
        stages{
                stage('clone and compile')
                    steps {
                        git branch 'declartive', url:'https://github.com/dumrepo/game-of-life.git'
                        sh 'mvn compile'
                    }
                }
        }
}
