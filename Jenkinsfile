pipeline {
  agent any
  stages {
    stage('Make') {
      steps {
          sh 'make -C examples/peripheral/blinky/pca10040/blank/armgcc/'
      }
    }
    stage('Archiving') {
      steps {
        archiveArtifacts artifacts: 'examples/peripheral/blinky/pca10040/blank/armgcc/_build/*.hex', onlyIfSuccessful: true
	archiveArtifacts artifacts: 'examples/peripheral/blinky/pca10040/blank/armgcc/_build/*.hex', onlyIfSuccessful: true
      }
    }
  }
}
