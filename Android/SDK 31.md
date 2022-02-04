<details>
    <summary>30.0.3</summary>
    
    1. API LEVEL 변경
       Tool - SDK Manager - 30.0.3 설치
       
    2. build.gradle (Module) 변경
       compileSdkVersion 30
       buildToolsVersion "30.0.3"
       targetSdkVersion 30

</details>

<details>
    <summary>d8 -> dx</summary>
    
    1. dx.bat 추가
       Android\Sdk\build=tools\31.0.0\dx.bat 생성 (30.0.3 폴더에서 복붙)
       (d8.bat의 파일명을 변경해도 된다고 함)
     
    2. dx.jar 추가
       Android\Sdk\build=tools\31.0.0\lib\dx.jar 생성 (30.0.3 폴더에서 복붙)
       (d8.bat의 파일명을 변경해도 된다고 함)
       
    3. android:exported 추가 명시
       AndroidManifest.xml에 <activity android:name=".MainActivity" android:exported="true">로 변경
       (android:exported="true" 추가)

</details>
