pipeline {
    agent any     
    stages {
        stage('Build') {
            steps {
              sh """
              #!/bin/bash
              packer validate GI_Pckr.json
              packer build GI_Pckr.json
              """
            }
        }
      }
    }
