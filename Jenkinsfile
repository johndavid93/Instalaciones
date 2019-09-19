node {
  stage('JIRA') {
    def testIssue = [fields: [ // id or key must present for project.
                               project: [id: '10100'],
                               summary: 'New JIRA Created from Jenkins.',
                               description: 'New JIRA Created from Jenkins.',
                               customfield_1000: 'customValue',
                               // id or name must present for issuetype.
                               issuetype: [id: '5']]]

    response = jiraEditIssue idOrKey: 'PRUEB', issue: testIssue

    echo response.successful.toString()
    echo response.data.toString()
  }
}
