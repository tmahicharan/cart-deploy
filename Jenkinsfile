@Library('jenkins-shared-library') _

// These receive parameters from jenkins CI. see nodeJSEKSPipeline
properties([
  parameters([
    string(name: 'appversion', defaultValue: ''),
    string(name: 'deploy_to', defaultValue: 'dev')
  ])
])

def configMap = [
    project: "roboshop",
    component: "cart",
    appversion: (params.appversion),
    deploy_to: (params.deploy_to)
]

EKSDeploy(configMap)