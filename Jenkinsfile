node
{

stage('runpython'){
   dir('validation') {
          sh "ls pythonscript/*.py|xargs -n 1 -P 4 python"
        }
    
}
}
