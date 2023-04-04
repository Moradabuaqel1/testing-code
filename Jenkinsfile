pipeline {
  agent any
  stages {
    stage ('test') {
      steps {
        echo "hello"
        slackSend botUser: true,
                 channel: '#new-jenkins-alerts',
                 color: '#00ff00',
                 message: 'Testing Jekins with Slack',
                 tokenCredentialId: 'slack-int'
      }
    }
  }
}
