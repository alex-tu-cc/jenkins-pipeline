pipeline {
    agent none
    stages {
        stage('alpine') {
            agent {
                docker {
                    label 'docker'
                    image 'maven:3-alpine'
                }
            }
            steps {
                sh 'cat /etc/*-release'
            }
        }
        stage('ubuntu') {
            agent {
                docker {
                    label 'docker'
                    image 'ubuntu:18.04'
                }
            }
            steps {
                sh 'cat /etc/*-release'
            }
        }
        stage('archlinux') {
            agent {
                docker {
                    label 'docker'
                    image 'archlinux/base'
                }
            }
            steps {
                sh 'cat /etc/*-release'
            }
        }
    }
}
