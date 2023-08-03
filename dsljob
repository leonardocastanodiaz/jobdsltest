// Example Job DSL Script to Create Folder and Pipeline Inside
folder('DSLJobs') {
    description('This is a sample folder')
    
    pipelineJob('DSLJobs/MyPipelineJob') {
        definition {
            cps {
                script("""
                    pipeline {
                        agent any
                        stages {
                            stage('Build') {
                                steps {
                                    echo 'Building...'
                                }
                            }
                            stage('Test') {
                                steps {
                                    echo 'Testing...'
                                }
                            }
                            stage('Deploy') {
                                steps {
                                    echo 'Deploying...'
                                }
                            }
                        }
                    }
                """)
            }
        }
    }
}
