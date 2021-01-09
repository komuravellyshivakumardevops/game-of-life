
node
{
   stage('cloning code')
    {
      git 'https://github.com/wakaleo/game-of-life.git'
    }
   stage('creating arfifacts')
   {
     sh 'mvn package'
   }
   stage('archiving artifacts')
    {
       archiveArtifacts artifacts: '/var/lib/jenkins/workspace/gameoflifeproj/gameoflife-      web/target', followSymlinks: false
    }
}


