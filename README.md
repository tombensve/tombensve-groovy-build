# POM to import using:

    <dependencyManagement>
        <dependencies>
            <dependency>
                <groupId>io.github.tombensve</groupId>
                <artifactId>tombensve-groovy-build</artifactId>
                <version>1.0.11</version>
                <scope>import</scope>
                <type>pom</type>
            </dependency>   
        </dependencies>
    </dependencyManagement> 

Note that the "11" in third version digit is the byte code level produced!

At the moment there is only byte code 11 available! I have 0 interest in 
wasting my time on figuring out problems arising from non backwards 
compatible JDK versions!! 

As of writing this I no longer work (health reasons), I now only code on my hobby projects at 
GitHub. And **MY time** is important to me! 

As of 2023 when I stopped working (as a consultant), no java project I've worked
on ever passed bytecode 11! 

This said, I do use the third version digit to specify bytecode level of compiled binary.
Groovy allows compiler to produce bytecode for newer bytecode versions. This only if
newer JVM versions will not run 11 bytecode. 
