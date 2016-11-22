node {
    stage('Build and import') {
                checkout scm  
                mvn 'versions:set -DnewVersion=1.1.1'
                mvn 'clean install xldeploy:import'
    }
}

def mvn(args) {
    sh "mvn ${args}"
}
