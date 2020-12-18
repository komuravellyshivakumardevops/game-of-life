

node
{
   stage('scm')
    {
      git 'https://github.com/wakaleo/game-of-life.git'
    }
   stage('creating arfifacts')
   {
     sh 'mvn package'
   }
}


