pipeline {
  agent any
  stages {
    stage ('build') {
      steps {	
	sh 'javac -d . src/.java'
	sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
	sh 'jar -cmvf MANIFEST.MF rectangle.jar .class'
      }
    }
  }
}
