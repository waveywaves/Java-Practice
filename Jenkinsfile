try {
    timeout(time: 20, unit: 'MINUTES') {
        def appName="webscraper--plugin"
        def project=""
        node {
            stage("Initialize") {
                project = env.PROJECT_NAME
            }
        }
        node("maven") {
            environment{
                MAVEN_MIRROR_URL = "https://repository.jboss.org/"
            }
            stage("Checkout") {
                git url: "https://github.com/waveywaves/Java-Practice", branch: "master"
            }
            stage("Build WAR") {
                sh "mvn clean package"
            }
        }
    }
} catch (err) {
    echo "in catch block"
    echo "Caught: ${err}"
    currentBuild.result = 'FAILURE'
    throw err
}