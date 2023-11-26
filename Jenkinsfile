// pipeline {
//
//       agent {
//           node { label 'Workstation'
//       }
//
//       stages {
//              stage('code checkout') {
//                  steps {
//                      git "https://github.com/saikumarsooda2/catalogue.git "
//                  }
//              }
//
// //     stages {
// //         stage ('Code checkout') {
// //             steps {
// //               echo 'Code checkout'
// //             }
// //         }
//
//         stage ('Build') {
//                     steps {
//                       echo 'Build'
//                     }
//                 }
//
//         stage ('Unit test') {
//                     steps {
//                       echo 'Unit test'
//                     }
//                 }
//
//         stage ('Code Analysis') {
//                     steps {
//                       echo 'Code Analysis'
//                     }
//                 }
//
//         stage ('Security Scanning') {
//                     steps {
//                       echo 'Security Scanning'
//                     }
//                 }

pipeline {
    agent { node { label 'Workstation' } }

    environment {
    SSH = credentials('SSH')
    }
     options {
            ansiColor('xterm')
      }

    stages {
        stage('Hello') {
      input {
        message "should we continue?"
        ok "we should"
        parameters {
        string(name: 'PERSON', defaultValue: 'Enter Your Name please', description: 'Hello Mr shall we run')
        }
      }
            steps {
                echo 'Hello World'
                sh 'env'
            }
        }
    }

   post {
        always {
            echo 'I will always say Hello again!'
        }
    }
}