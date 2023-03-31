pipeline {
    agent any
    parameters {
        string(name: 'TOPIC_NAME', defaultValue: 'DevOps', description: 'Topics to learn')
        string(name: 'TARGET', defaultValue: 'Dream-Job', description: 'Target goal')
    }

    stages {
        //stage('Clone Repo') {
        //    steps {
        //        checkout scm
        //    }
        //}
        stage('Call Script') {
            steps {
                sh 'chmod +x shellScript.sh'
                sh '/shellScript.sh ${TOPIC_NAME} ${TARGET}'
            }
        }
    }
}
