# POM to import using:

    <dependencyManagement>
        <dependencies>
            <dependency>
                <groupId>io.github.tombensve</groupId>
                <artifactId>tombensve-groovy-build</artifactId>
                <version>1.0.0-BC11</version>
                <scope>import</scope>
                <type>pom</type>
            </dependency>   
        </dependencies>
    </dependencyManagement> 

Or specify as parent!

This is my new version standard for my projects. 

At the moment there is only byte code 11 available! Personally I have no interest in
going above 11 for my Github code. I'm doing this because it is fun! Chasing things 
that no longer work in 12+ is not included in my definition of fun! 

That said most of my GitHub code is not done in Java, but in Groovy, and I stick 
with Groovy solutions for different things. Groovy can produce bytecode for higher
versions Java level, and I might produce higher bytecode versions from my Groovy
code, as long as I don't have to adapt my code to do so!
