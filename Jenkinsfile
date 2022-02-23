pipeline {
    agent any 
    environment {
            "client_id": "f8aa5f4b-615b-46dc-8538-9626294a7d19"
            "client_secret": "2Yv7Q~hIjFYXUKpnwKGvdi~Rz146al1fXoOAl"
            "tenant_id": "57a05638-7606-4e30-8662-135f1967a8d0"
            "subscription_id": "f2a62f2c-86fc-4221-b813-cd041ddbf8e5" 
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
