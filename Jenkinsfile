pipeline {
         agent any
         stages {
                 stage('Clone repository') {
                    steps {
                        echo 'Cloning repository...'
                        script{
                        checkout scm
                        }
                    }
                 }

                 stage('Build') {
                 steps {
                    script{
                        app = docker.build("test")
                    }
                 }
                 }
              }
}
