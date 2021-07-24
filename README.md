# install JDK in Ubuntu
  # [oracle JDK & JRE](#oracle)
  # [open JDK & JRE](#open)
## Oracle
Download Letest JDK from <h1 align=center>[Oracle ⇩](https://www.oracle.com/java/technologies/javase-downloads.html) in Tar.GZ format</h1>
+ Step 1 :
  - Make Java Virtual Machine (JVM) Directory 
  ```bash
  sudo mkdir -p /usr/lib/jvm
  ```
+ Step 2 :
  - Extract Downloaded Tar.GZ file 
  ```bash
  sudo tar zxvf /Downloads/jdk-`VERSION`_`OS_VERSION `_bin.tar.gz -C /usr/lib/jvm
  ```
+ Step 3 : Install JDK 
  - java
  ```bash
  sudo update-alternatives --install "/usr/bin/java" "java" "/usr/lib/jvm/jdk-`VERSION`/bin/java" 1
  ```
  - javac
  ```bash
  sudo update-alternatives --install "/usr/bin/javac" "javac" "/usr/lib/jvm/jdk-`VERSION`/bin/javac" 1
  ```
+ Step 4 : Set JDK
  - java
  ```bash
  sudo update-alternatives --set java /usr/lib/jvm/jdk-`VERSION`/bin/java
  ```
  - javac
  ```bash
  sudo update-alternatives --set javac /usr/lib/jvm/jdk-`VERSION`/bin/javac
  ```
## Open
### `VERSION`: `8` / `11` / `13` / `14` / `16`
+ Step 1 :
  - JDK
  ```bash
  sudo apt install openjdk-`VERSION`-jdk -y
  ```
  - JRE
  ```bash
  sudo apt install openjdk-`VERSION`-jre -y
  ```
### Select Alternative Version
+ java
  ```bash
  sudo update-alternatives --config java
  ```
+ javac
  ```bash
  sudo update-alternatives --config javac
  ```
### Verify / Check Version 
+ java
  ```bash
  java --version
  ```
+ javac
  ```bash
  javac --version
  ```
***
