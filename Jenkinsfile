pipeline {
  agent any
  stages {
    stage('Make') {
      steps {
          sh 'make -C examples/peripheral/blinky/pca10036/blank/armgcc/'
      }
    }
    stage('Archiving') {
      steps {
        archiveArtifacts artifacts: 'examples/peripheral/blinky/pca10036/blank/armgcc/_build/*.hex', onlyIfSuccessful: true
      }
    }
  }
}