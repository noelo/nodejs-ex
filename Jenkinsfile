node('node') {
stage 'tag'
openshiftTag(namespace: 'development', sourceStream: 'nodejs-example', sourceTag: 'latest', destinationNamespace: 'testing', destinationStream: 'nodejs-example', destinationTag: 'latest')
stage 'deploy'
openshiftDeploy(deploymentConfig: 'nodejs-example', namespace: 'testing')
}
