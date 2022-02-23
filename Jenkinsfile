pipeline {
    agent any     
    stages {
        stage('Build') {
            steps {
              sh """
              #!/bin/bash
              packer init .
              packer validate 
              packer build -force .
              """
            }
        }
      }
    }
