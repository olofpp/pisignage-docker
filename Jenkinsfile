#!/usr/bin/env groovy
node {

  // Global variables
  def STACK_NAME="pisignage"

  // Get the latets code
  stage('Checkout Git Repository') {
    checkout scm
  }

  // Deploy the new image
  stage('Deploy piSignage') {
        sh "docker-compose -f docker-compose-traefik.yml up -d"
  }
}
