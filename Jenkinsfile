
node {
 /*/  unclassified:
  jiraStepsConfig:
    sites:
      name: 'jira'
      url: 'http://192.168.200.52:8085'
      timeout: 10000
      readTimeout: 10000
      loginType: 'BASIC'
      userName: 'jhon.bejarano'
      password: 'krathos26'
      /*/
    
  stage('JIRA') {
   /*/ def testIssue = [fields: [ // id or key must present for project.
                               project: [id: '10100'],
                               summary: 'New JIRA Created from Jenkins.',
                               description: 'New JIRA Created from Jenkins.',
                               customfield_1000: 'customValue',
                               // id or name must present for issuetype.
                               issuetype: [id: '5']]]

    response = jiraEditIssue idOrKey: 'PRUEB', issue: testIssue

    echo response.successful.toString()
    echo response.data.toString()
    /*/
    
    def issue = [fields: [ project: [key: 'PRUEB'],
                           // id or key must present for project.
                               project: [id: '10100'],
                       summary: 'New JIRA Created from Jenkins.',
                       description: 'New JIRA Created from Jenkins.',
                            issuetype: [name: 'Task']]]
/*/ def newIssue = jiraNewIssue issue: issue, site: 'jira'
echo newIssue.data.key /*/
  }
}
