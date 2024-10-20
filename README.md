# POM to inherit from to be able to build groovy code. 

Soince I'm writing more Groovy code than Java code, I have configured this pom
with everything I need to build my Groovy projects. I just specify this as
parent of my projects and I don't have to set everything up nor copy + paste.

    <parent>
        <groupId>com.github.tombensve</groupId>
        <artifactId>groovy-build</artifactId>
        <version>1.0.11</version>
    </parent>

Note that the "11" in third version digit is the byte code level produced!

At the moment there is only byte code 11 available! I have 0 interest in 
wasting my time on figuring out problems arising from non backwards 
compatible JDK versions!! 

I do use the third version digit to specify bytecode level of compiled binary.
Groovy allows compiler to produce bytecode for newer bytecode versions. This only if
newer JVM versions will not run 11 bytecode. 
