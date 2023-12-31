# build-wrapper-linux-x86

## Download and unzip the Build Wrapper for Linux

```bash
curl -sSLo /opt/build-wrapper-linux-x86.zip https://github.com/shenxianpeng/build-wrapper-linux-x86/raw/main/build-wrapper-linux-x86.zip
cd /opt && unzip build-wrapper-linux-x86.zip
export PATH=/opt/build-wrapper-linux-x86:$PATH
```

## Execute the Build Wrapper as a prefix to your build command

Run the following command in your project's folder.

```bash
build-wrapper-linux-x86-64 --out-dir bw-output <your clean build command>
```

Please visit the [official documentation](https://docs.sonarqube.org/9.9/analyzing-source-code/languages/c-family/) of the Build Wrapper for more details.


>**Note**
>
>If you have trouble using the build wrapper, you can try using a [compilation database](https://docs.sonarqube.org/9.9/analyzing-source-code/languages/c-family/).
>
>You can also speed up your analysis by enabling [multi-threading and caching](https://docs.sonarqube.org/9.9/analyzing-source-code/languages/c-family/#analysis-cache).

## Download SonarScanner for Linux

Version 4.8 (2022-02-06)

https://binaries.sonarsource.com/Distribution/sonar-scanner-cli/sonar-scanner-cli-4.8.0.2856-linux.zip

Verify your installation by opening a new shell and executing the command `sonar-scanner -h`, You should get output like this:

```bash
usage: sonar-scanner [options]

Options:
-D,--define <arg>     Define property
-h,--help             Display help information
-v,--version          Display version information
-X,--debug            Produce execution debug output
```
