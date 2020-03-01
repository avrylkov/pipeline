pipeline {
  agent any
  
  environment {
        APP_NAME = "bar"
    }
  
  stages {
        /**
         * the stage directive should contain a steps section, an optional agent section, or other stage-specific directives
         * all of the real work done by a Pipeline will be wrapped in one or more stage directives
         */
        stage('Prepare') {
            steps {
              echo "git checkout"
              echo "You can also use BUILD_NUMBER -> ${BUILD_NUMBER}"
              echo "APP_NAME = ${env.APP_NAME}"
              bat  "echo I can access $BUILD_NUMBER in shell command as well."
              git branch: 'master',
                  url: 'https://github.com/avrylkov/demo-gradle.git'            
              bat "dir"
            }
         }
      }    
}
