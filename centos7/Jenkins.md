1.
sudo yum update

2. 타임존 변경
sudo rm /etc/localtime
sudo ln -s /usr/share/zoneinfo/Asia/Seoul /etc/localtime

3. Host 네임 변경

4. wget  설치
sudo yum install wget

5. IP 고정


# 6. 자바 설치

```
yum install java-1.8.0-openjdk-devel.x86_64
```

자바 환경변수 설정


위치 확인
```
readlink -f /usr/bin/javac
```

위치 예시
```
/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.161-0.b14.el7_4.x86_64
```

여기 열어서 수정
```
vi /etc/profile
```

문구 예시
```
export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.161-0.b14.el7_4.x86_64
```

```
source /etc/profile
```

확인
```
echo $JAVA_HOME
```


https://blog.jiniworld.me/88

7. 깃
https://linuxize.com/post/how-to-install-git-on-centos-7/

7. 톰캣
https://linuxize.com/post/how-to-install-tomcat-9-on-centos-7/
https://linuxize.com/post/how-to-install-tomcat-8-5-on-centos-7/

7. 메이븐 설치
https://linuxize.com/post/how-to-install-apache-maven-on-centos-7/

7. 젠킨스 설치
https://www.vultr.com/docs/how-to-install-jenkins-on-centos-7


# 자바
export JAVA_HOME=/usr/lib/jvm/java-1.8.0-openjdk-1.8.0.292.b10-1.el7_9.x86_64

#메이븐
export MAVEN_HOME=/usr/share/maven

PATH=$PATH:$JAVA_HOME/bin:$MAVEN_HOME/bin
export PATH

마리아 DB
https://linuxize.com/post/install-mariadb-on-centos-7/

















