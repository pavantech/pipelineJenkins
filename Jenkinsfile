node
{
stage('checkout')
   {
      checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/pavantech/pipelineJenkins.git']]])
   }
stage('runpython'){
   dir('validation') {
          sh "ls pythonscript/*.py|xargs -n 1 -P 4 python"
        }
    
}
}
