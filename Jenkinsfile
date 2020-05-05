node('JS 02') {
    stage('GIT CLONE'){
        git 'https://github.com/wakaleo/game-of-life.git'
    }
    stage('build tool maven compile'){
        sh 'mvn compile'
    }
    stage('build tool maven test'){
        sh 'mvn test'
    }
    stage('build tool maven package'){
        sh 'mvn package'
    }
    stage('archive artifacts'){
        archive 'gameoflife-web/target/game*.war'
    }
    stage('archive test results'){
        junit 'gameoflife-web/target/surefire/*'
    }
}