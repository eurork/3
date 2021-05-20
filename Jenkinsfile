pipeline {
    agent any;
    stages{
      stage('deploy') {
        steps {
          sh 'echo "rozpoczynam deploy . . ."'
          sh 'sleep 1'
          copyArtifacts filter: 'test.zip', fingerprintArtifacts: true, projectName: 'build'
          unzip zipFile: 'test.zip', dir: './archive_new'
          sh 'cd archive_new'
          sh 'rm plik.sh plik2.py plik3.rpm plik4.rpm'
          sh 'ls -al'
          sh 'echo "Deploy zakonczony prawidlowo."'
        }
      }
    }
}