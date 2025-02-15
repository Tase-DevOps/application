@Library('tase-shared-library')_

pipeline {
    agent any

    stages {
        stage('Prepare Environment') {
            steps {
                checkout scm
                echo 'Hello World'
                prepareEnv script: this, action: 'get', job_parameter: 'git_committer'
            }
        }
        stage('Build'){
            steps {
                echo 'Build Application'
            }
        }      
        stage('Test'){
            steps {
                echo 'Tests'
            }
        }      
        stage('Package'){
            steps {
                echo 'package'
            }
        }      
        stage('Upload'){
            steps {
                echo 'upload'
            }
        }      
        stage('Post Action job'){
            steps {
                echo 'Post Action'
            }
        }      
    }
}
