node {
    stage('Deploy') {
        sh 'cd ..'
        sh 'echo "rozpoczynam deploy . . ."'
        sh 'sleep 1'
        sh 'rm plik.sh plik2.py plik3.rpm plik4.rpm'
        sh 'sleep 1'
        sh 'ls -al'
        sh 'echo "Deploy zakonczony prawidlowo"'
    }
}
// pipeline {
//     agent any
//     stages {
//         stage('Deploy') {
//             steps {
//                 echo "rozpoczynam deploy . . ."
//                 sleep 2
//                 rm plik.sh plik2.py plik3.rpm plik4.rpm
//                 sleep 1
//                 echo "koncze deploy."
//             }
//         }
//     }
// }