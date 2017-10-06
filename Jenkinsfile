@Library('sharedLibrary') _

StandardPipeline {
                //Tools
                Maven_tool = "Maven 3.3.9"
                Java_tool = "JAVA_8"

                //Build Parameters
    SCM_url = "https://conexus.prod.fedex.com:9443/subversion/fxf_sp_index_web_gui/branches/Maven_Conversion/Entry_OFS_Maven"
    MVN_build = "clean compile test site package -s settings.xml"
    SonarQube_Analysis = "sonar:sonar -Dmaven.test.skip=true -s settings.xml"
    Nexus_Deploy = "deploy -Dmaven.test.skip=true -s settings.xml"

                //Junit parameters
                junit_path = "target/surefire-reports/**/*.xml"

                //FindBugs Parameters
                findbugs_failedTotalHigh = "10"
    findbugs_failedTotalLow = "60"
    findbugs_failedTotalNormal = "198"
    findbugs_healthy = "90"
    findbugs_pattern = "**/findbugsXml.xml"
    findbugs_unHealthy = "10"
    findbugs_unstableTotalHigh = "10"
    findbugs_unstableTotalLow = "60"
    findbugs_unstableTotalNormal = "198"

    //Checkstyle Parameters
    checkstyle_failedTotalAll = "22463"
    checkstyle_failedTotalHigh = "22463"
    checkstyle_failedTotalLow =  "22463"
    checkstyle_failedTotalNormal =  "5"
    checkstyle_healthy = "90"
                checkstyle_pattern = "**/checkstyle-result.xml"
    checkstyle_unHealthy = "22463"
    checkstyle_unstableTotalAll = "22463"
    checkstyle_unstableTotalHigh = "22463"
    checkstyle_unstableTotalLow = "22463"
    checkstyle_unstableTotalNormal = "4"

    //PMD Parameters
    PMD_healthy = "90"
                PMD_pattern = "**/target/pmd.xml"
    PMD_unHealthy = "20"
    PMD_unstableTotalHigh = "90"
    PMD_unstableTotalLow = "20"
    PMD_unstableTotalNormal = "280"
}
