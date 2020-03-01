pipeline {
  agent any
  stages {
        /**
         * the stage directive should contain a steps section, an optional agent section, or other stage-specific directives
         * all of the real work done by a Pipeline will be wrapped in one or more stage directives
         */
        stage('Prepare') {
            steps {
              git branch: 'master',
                  url: 'https://github.com/avrylkov/demo-gradle.git'            
            }
         }
      }    
}
