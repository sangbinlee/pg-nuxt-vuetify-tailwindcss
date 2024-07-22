pipeline {
    agent any
    stages {
        stage('Clone Sources') {
          steps {
            echo 'landing2 building the application...'
            // git 'https://gitlab.com/chiminyau/ci-test.git'
          }
        }
        stage('Information') {
          steps {
            echo 'landing2 Information...'
            sh 'node -v'
            sh 'npm -v'
          }
        }
        stage('Config') {
          steps {
            echo 'landing2 Config...  now....'
            // sh 'npm set registry https://registry.npm.taobao.org'
            // sh 'npm set disturl https://npm.taobao.org/dist'
            // sh 'npm set chromedriver_cdnurl http://cdn.npm.taobao.org/dist/chromedriver'
            // sh 'npm set operadriver_cdnurl http://cdn.npm.taobao.org/dist/operadriver'
            // sh 'npm set phantomjs_cdnurl http://cdn.npm.taobao.org/dist/phantomjs'
            // sh 'npm set fse_binary_host_mirror https://npm.taobao.org/mirrors/fsevents'
            // sh 'npm set sass_binary_site http://cdn.npm.taobao.org/dist/node-sass'
            // sh 'npm set electron_mirror http://cdn.npm.taobao.org/dist/electron/'
          }
        }
        stage('Dependencies') {
          steps {
            sh 'npm install'
          }
        }
        // stage('Unit Test') {
        //   steps {
        //     sh 'npm run unit'
        //   }
        // }
        stage('Build') {
          steps {
            echo 'landing2 building the application...  now....'
            sh 'npm run build'
          }
        }
        // stage('build') {
        //     steps {
        //         echo 'building the application...'
        //         cd "/var/jenkins_home/workspace/Book Management App/src/frontend"
        //         yarn install
        //         yarn clean
        //         yarn build
        //     }
        // }
        stage('test') {
            steps {
                echo 'landing2 testing the application...'
            }
        }
        stage('deploy') {
            steps {
                echo 'landing2 deploying the application...'
            }
        }
    }
}
