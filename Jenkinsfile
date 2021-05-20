pipeline {
    agent any
    environment {
      VERSION = '1.0'
    }
    stages{
      stage('deploy') {
        steps {
          sh 'echo "rozpoczynam deploy . . ."'
          sh 'sleep 1'
          copyArtifacts filter: 'test.zip', fingerprintArtifacts: true, projectName: "build-${VERSION}"
          unzip zipFile: 'test.zip', dir: '.'
          sh 'rm plik.sh plik2.py plik3.rpm plik4.rpm'
          sh 'ls -al'
          sh 'echo "Deploy zakonczony prawidlowo."'
        }
      }
    }
}