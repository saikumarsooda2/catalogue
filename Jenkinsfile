pipeline {

      agent {
          node { label 'Workstation'
      }

      stages {
             stage('code checkout') {
                 steps {
                     git "https://github.com/saikumarsooda2/catalogue.git "
                 }
             }

//     stages {
//         stage ('Code checkout') {
//             steps {
//               echo 'Code checkout'
//             }
//         }

        stage ('Build') {
                    steps {
                      echo 'Build'
                    }
                }

        stage ('Unit test') {
                    steps {
                      echo 'Unit test'
                    }
                }

        stage ('Code Analysis') {
                    steps {
                      echo 'Code Analysis'
                    }
                }

        stage ('Security Scanning') {
                    steps {
                      echo 'Security Scanning'
                    }
                }