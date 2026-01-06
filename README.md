
# GraalVM

GraalVM JDK an advanced JDK that acts as a high-performance "super-runtime" for Java. It is designed to modernize how applications run, particularly in cloud and microservices environments. Traditional JVMs (like OpenJDK) rely on Just-In-Time (JIT) compilation, which optimizes code while it runs. GraalVM adds a powerful alternative: Ahead-of-Time (AOT) compilation via Native Image.

What is Native Image?

It is standalone, executable binary created by AoT (ahead of time) compiling Java code into machine code, liberating the dependency of JVM at runtime resulting in instant start up. 


- without native image
![GraalVM Screenshot](https://github.com/gagaci/asset/blob/main/Screenshot%202026-01-06%20at%2015.05.49.png?raw=true)

    0.319 seconds

- with native image 
![GraalVM Screenshot](https://github.com/gagaci/asset/blob/main/Screenshot%202026-01-06%20at%2015.05.57.png?raw=true)

    0.016 seconds




## Try Locally

Clone the project

```bash
  git clone https://link-to-project
```

Convert to native image

```bash
  ./mvnw -Pnative native:compile -DskipTests 
```

Run the image

```bash
  ./target/my-project
```

## Resource

 - [Graalvm youTube](https://youtu.be/sI-zXYLKzfk?si=Z1ZOkhdWHumEAij4)
 - [demo project youTube](https://youtu.be/FjRBHKUP-NA?si=8exUOJGHByMnFHSL) 

## 📜 License

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](https://choosealicense.com/licenses/mit/)
