# learningMaven
I am learning Maven using following links :

https://www.tutorialspoint.com/maven

https://www.google.com/search?ei=sXkvXJaQKtLIaJqbgMgF&q=how+to+run+mvn+clean+package+in+eclipse&oq=run+mvn+clean+package+on+eclipse&gs_l=psy-ab.1.0.0i13i5i30.8389.12560..16898...0.0..0.117.598.6j1......0....1..gws-wiz.......0i71j35i304i39j0i7i30i19j0i7i30j0i30.i1OezszdXUw

https://docs.aws.amazon.com/lambda/latest/dg/java-create-jar-pkg-maven-and-eclipse.html

http://www.vogella.com/tutorials/EclipseMaven/article.html

https://stackoverflow.com/questions/19793895/run-mvn-clean-install-in-eclipse

https://www.google.com/search?q=no+compiler+is+provided+in+this+environment.+perhaps+you+are+running+on+a+jre+rather+than+a+jdk+cmd&oq=No+compiler+is+provided+in+this+environment.+Perhaps+you+are+running+on+a+JRE+rather+than+a+JDK%3F&aqs=chrome.1.69i57j0.5253j0j7&sourceid=chrome&ie=UTF-8

https://stackoverflow.com/questions/22721283/maven-commandline-no-compiler-is-provided-in-this-environment

https://crunchify.com/mavenmvn-clean-install-update-project-and-project-clean-options-in-eclipse-ide-to-fix-any-dependency-issue/

Learning windows commands

https://www.commentcamarche.net/faq/13047-invite-de-commande-cmd-sous-windows-10-8-et-7

I get this error :

"no compiler is provided in this environment. perhaps you are running on a jre rather than a jdk cmd"

So I need to change my system variable. 

I succeed, thanks to https://stackoverflow.com/questions/22721283/maven-commandline-no-compiler-is-provided-in-this-environment

I get this error : "java.lang.NoClassDefFoundError: org/apache/maven/doxia/siterenderer/DocumentContent" while generating the site of
my maven project

https://stackoverflow.com/questions/51091539/maven-site-plugins-3-3-java-lang-classnotfoundexception-org-apache-maven-doxia

https://stackoverflow.com/questions/2555845/how-to-update-maven-repository-in-eclipse/24509023

https://maven.apache.org/guides/introduction/introduction-to-the-lifecycle.html

To solve the problem about mvn site, I add this to pom.xml 

```

<reporting>
    <plugins>
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-project-info-reports-plugin</artifactId>
            <version>3.0.0</version>
            <reportSets>
                <reportSet>
                    <reports>
                        <report>index</report>
                        <report>licenses</report>
                        <report>dependency-info</report>
                    </reports>
                </reportSet>
            </reportSets>
        </plugin>
    </plugins>
</reporting>

<build>
    <plugins>
        <!-- Part of Maven - specified version explicitly for compatibility
             with the maven-project-info-reports-plugin 3.0.0-->
        <plugin>
            <groupId>org.apache.maven.plugins</groupId>
            <artifactId>maven-site-plugin</artifactId>
            <version>3.7.1</version>
        </plugin>
    </plugins>
</build>

```

GIT MAVEN

http://objis.com/tutoriel-integration-git-maven/

https://maven.apache.org/scm/git.html

developerconnection github

https://www.google.com/search?q=developerconnection+github&oq=developerConnection&aqs=chrome.5.69i57j0l5.8751j0j7&sourceid=chrome&ie=UTF-8

https://github.com/kevinsawicki/github-maven-example/blob/master/example/pom.xml

Finding maven settings.xml file for maven eclipse

https://www.google.com/search?q=settings.xml+maven+eclipse&oq=settings.xml+maven+&aqs=chrome.4.69i57j0l5.24584j1j7&sourceid=chrome&ie=UTF-8

https://stackoverflow.com/questions/4626609/maven-plugin-in-eclipse-settings-xml-file-is-missing

http://maven.apache.org/settings.html

https://github.com/kevinsawicki/github-maven-example

https://www.google.com/search?q=maven+release+plugin+scm+comment+prefix&oq=%3CscmCommentPrefix%3E&aqs=chrome.2.69i57j0l3.11682j0j7&sourceid=chrome&ie=UTF-8


I get this error while running mvn clean install (git deployment)

https://www.google.com/search?q=an+api+incompatibility+was+encountered+while+executing&oq=An+API+&aqs=chrome.2.69i57j69i60j0l4.33601j1j7&sourceid=chrome&ie=UTF-8

https://www.google.com/search?q=failed+to+execute+goal+com.github.github%3A+downloads-maven-plugin%3A0.6%3Aupload&oq=failed+to+execute+goal+com.github.github%3A+downloads-maven-plugin%3A0.6%3Aupload&aqs=chrome..69i57.107082j0j7&sourceid=chrome&ie=UTF-8

https://github.com/github/maven-plugins/issues/41

https://maven.apache.org/plugins/maven-project-info-reports-plugin/

## how to get all archetypes maven in eclipse

https://www.google.com/search?q=how+to+get+all+archetypes+maven+in+eclipse&oq=how+to+get&aqs=chrome.1.69i57j69i59j35i39j0l3.10923j1j7&sourceid=chrome&ie=UTF-8

https://howtodoinjava.com/eclipse/how-to-import-maven-remote-archetype-catalogs-in-eclipse/

## Maven POM reference

https://maven.apache.org/pom.html

## why is it important to get a license for a open source project ?

https://www.google.com/search?q=why+is+it+important+to+get+a+license+for+a+open+source+project+%3F&oq=why+is+it+important+to+get+a+license+for+a+open+source+project+%3F&aqs=chrome..69i57.34456j0j7&sourceid=chrome&ie=UTF-8

https://medium.com/@apondihazel/the-importance-of-an-open-source-license-and-how-to-add-one-to-your-project-cf0f8cd6d806










