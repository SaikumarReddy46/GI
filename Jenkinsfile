pipeline {
    agent any 
    environment {
            ARM_CLIENT_ID = "f8aa5f4b-615b-46dc-8538-9626294a7d19"
            ARM_CLIENT_SECRET = "2Yv7Q~hIjFYXUKpnwKGvdi~Rz146al1fXoOAl"
            ARM_TENANT_ID = "57a05638-7606-4e30-8662-135f1967a8d0"
            ARM_SUBSCRIPTION_ID = "f2a62f2c-86fc-4221-b813-cd041ddbf8e5"
    }
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
