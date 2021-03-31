## 유니티 AR Foundation을 이용한 Android 빌드 방법 정리
- Unity 2019.4.22f1 버전 이용
- AR Foundation을 이용한 안드로이드 빌드 방법

### 1. Window -> Package Manager
- AR Foundation 설치
- ARCore XP Plugin 설치

### 2. File -> Build Settings
- Android로 switch platform

### 3. File -> Build Settings -> Player Settings
- Player
>> Android 탭에서 Other Settings -> Graphics APIs -> Vulkan 제거
>> 
>> Minimum API Level : Android 7.0 'Nougat' 이상 설정
>> 
>> Publishing Settings -> Build -> Custom Main Gradle Template 체크
>> 
>> Publishing Settings -> Build -> Custom Launcher Gradle Template 체크
>> 

- XR Plug-in Management
>> Plug-in Providers -> ARCore 체크

### 4. Template 설정
- Project계층 -> Assets -> Plugins -> Android -> launcherTemplate 파일을 이 Repositories의 [Android -> Plugins -> launcherTemplate 파일 내용으로 수정]
- Project계층 -> Assets -> Plugins -> Android -> mainTemplate 파일을 이 Repositories의 [Android -> Plugins -> mainTemplate 파일 내용으로 수정]
