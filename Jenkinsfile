node('JS 2') {
    stage('git clone') {
    git 'https://github.com/rajeshande430/gol.git'
    }
    stage('package'){
    sh 'mvn package'
    }
    stage('artifacts archive')
    archive 'gameoflife-web/target/*.war'
}