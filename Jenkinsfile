node {
    stage('git clone') {
    git 'https://github.com/rajeshande430/gol.git'
    }
    stage('package'){
    bat label: '', script: 'mvn package'
    }
}