# Use Oracle JDK instead of the default openjdk that comes with maven
Run the below commands :
- Download .deb file and install it
- Run the below commands in your terminal
    > **NOTE** : Please change **jdk-20** to **"jdk-[your-java-version]"** before running these commands.
    ```bash
    sudo update-alternatives --install /usr/bin/jar jar /usr/lib/jvm/jdk-20/bin/jar 2000
    sudo update-alternatives --install /usr/bin/javac javac /usr/lib/jvm/jdk-20/bin/javac 2000
    sudo update-alternatives --install /usr/bin/jcmd jcmd /usr/lib/jvm/jdk-20/bin/jcmd 2000
    sudo update-alternatives --install /usr/bin/jdeprscan jdeprscan /usr/lib/jvm/jdk-20/bin/jdeprscan 2000
    sudo update-alternatives --install /usr/bin/jhsdb jhsdb /usr/lib/jvm/jdk-20/bin/jhsdb 2000
    sudo update-alternatives --install /usr/bin/jlink jlink /usr/lib/jvm/jdk-20/bin/jlink 2000
    sudo update-alternatives --install /usr/bin/jpackage jpackage /usr/lib/jvm/jdk-20/bin/jpackage 2000
    sudo update-alternatives --install /usr/bin/jshell jshell /usr/lib/jvm/jdk-20/bin/jshell 2000
    sudo update-alternatives --install /usr/bin/jstatd jstatd /usr/lib/jvm/jdk-20/bin/jstatd 2000
    sudo update-alternatives --install /usr/bin/rmiregistry rmiregistry /usr/lib/jvm/jdk-20/bin/rmiregistry 2000
    sudo update-alternatives --install /usr/bin/jarsigner jarsigner /usr/lib/jvm/jdk-20/bin/jarsigner 2000
    sudo update-alternatives --install /usr/bin/javadoc javadoc /usr/lib/jvm/jdk-20/bin/javadoc 2000
    sudo update-alternatives --install /usr/bin/jconsole jconsole /usr/lib/jvm/jdk-20/bin/jconsole 2000
    sudo update-alternatives --install /usr/bin/jdeps jdeps /usr/lib/jvm/jdk-20/bin/jdeps 2000
    sudo update-alternatives --install /usr/bin/jimage jimage /usr/lib/jvm/jdk-20/bin/jimage 2000
    sudo update-alternatives --install /usr/bin/jmap jmap /usr/lib/jvm/jdk-20/bin/jmap 2000
    sudo update-alternatives --install /usr/bin/jps jps /usr/lib/jvm/jdk-20/bin/jps 2000
    sudo update-alternatives --install /usr/bin/jstack jstack /usr/lib/jvm/jdk-20/bin/jstack 2000
    sudo update-alternatives --install /usr/bin/jwebserver jwebserver /usr/lib/jvm/jdk-20/bin/jwebserver 2000
    sudo update-alternatives --install /usr/bin/serialver serialver /usr/lib/jvm/jdk-20/bin/serialver 2000
    sudo update-alternatives --install /usr/bin/java java /usr/lib/jvm/jdk-20/bin/java 2000
    sudo update-alternatives --install /usr/bin/javap javap /usr/lib/jvm/jdk-20/bin/javap 2000
    sudo update-alternatives --install /usr/bin/jdb jdb /usr/lib/jvm/jdk-20/bin/jdb 2000
    sudo update-alternatives --install /usr/bin/jfr jfr /usr/lib/jvm/jdk-20/bin/jfr 2000
    sudo update-alternatives --install /usr/bin/jinfo jinfo /usr/lib/jvm/jdk-20/bin/jinfo 2000
    sudo update-alternatives --install /usr/bin/jmod jmod /usr/lib/jvm/jdk-20/bin/jmod 2000
    sudo update-alternatives --install /usr/bin/jrunscript jrunscript /usr/lib/jvm/jdk-20/bin/jrunscript 2000
    sudo update-alternatives --install /usr/bin/jstat jstat /usr/lib/jvm/jdk-20/bin/jstat 2000
    sudo update-alternatives --install /usr/bin/keytool keytool /usr/lib/jvm/jdk-20/bin/keytool 2000
    ```
- Done :tada:!
