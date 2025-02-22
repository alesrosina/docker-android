![GitHub Workflow Status](https://img.shields.io/github/workflow/status/beevelop/docker-android/Docker%20Image?style=for-the-badge)
![Docker Pulls](https://img.shields.io/docker/pulls/beevelop/android.svg?style=for-the-badge)
![Docker Stars](https://img.shields.io/docker/stars/beevelop/android?style=for-the-badge)
![Docker Image Size (tag)](https://img.shields.io/docker/image-size/beevelop/android/latest?style=for-the-badge)
![License](https://img.shields.io/github/license/beevelop/docker-android?style=for-the-badge)
[![GitHub release](https://img.shields.io/github/release/beevelop/docker-android.svg?style=for-the-badge)](https://github.com/beevelop/docker-android/releases)
![GitHub Release Date](https://img.shields.io/github/release-date/beevelop/docker-android?style=for-the-badge)
![CalVer](https://img.shields.io/badge/CalVer-YYYY.MM.MICRO-22bfda.svg?style=for-the-badge)
[![Beevelop](https://img.shields.io/badge/-%20Made%20with%20%F0%9F%8D%AF%20by%20%F0%9F%90%9Dvelop-blue.svg?style=for-the-badge)](https://beevelop.com)

# Android 11.0
### based on [beevelop/java](https://github.com/beevelop/docker-java)
- Java 8 (OpenJDK 1.8.0_282)
- Gradle 4.4.1 (Groovy: 2.4.16)
- Apache Maven 3.6.3
- Ant 1.10.7

### Pull, build or run this image
```bash
# pull the most recent tag / release
docker pull beevelop/android:v2021.06.2


# or run the image interactively
docker run --rm --name beevelop -it beevelop/android:v2021.06.2 bash

# or build the image from GitHub
docker build -t beevelop/android github.com/beevelop/docker-base
```

### Or use as base image
```Dockerfile
FROM beevelop/android:v2021.06.2
```

## Maintenance
- [Command Line Tools Download](https://developer.android.com/studio#span-idcommand-toolsa-namecmdline-toolsacommand-line-tools-onlyspan)
- List build-tools versions: `sdkmanager --sdk_root=${ANDROID_SDK_ROOT}  --list | grep build-tools`
- List platforms: `sdkmanager --sdk_root=${ANDROID_SDK_ROOT}  --list | grep 'platforms:'`

---

![Beevelop's Docker Image Hierarchy](https://gist.githubusercontent.com/beevelop/b0cddab7209a683c77560d06ff00bc8e/raw/15429ee1d02e2c4dc019b760ca8c7ceff5911b82/hierarchy.png)

---

### Use tags where possible, because...

![One does not simply use latest](https://i.imgflip.com/1fgwxr.jpg)
