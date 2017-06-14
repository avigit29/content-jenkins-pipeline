pipeline {
	agent any
	
	stages {
		stage('build'){
		steps{
			sh 'javac -d . src/*.java'
			sh 'echo Main-Class: Rectangulator > MANIFEST.MF'
			sh 'jar -cvfm MANIFEST.MF rectangle.jar *.class'
			}
		}
	}

}

