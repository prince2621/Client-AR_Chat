# Agora video with AR Core and Sceneform drawing integrated

1. Extracted Agora ARCore from Agora Sample Repository
2. Added Sceneform Drawing to it
3. Added the poject to firebase realtime Database

# How to use this

1. Create a developer account at agora.io. Once you finish the sign-up process, you are redirected to the dashboard.
2. Navigate in the dashboard tree on the left to Projects > Project List.
3. Locate the file app/src/main/res/values/strings.xml and replace <#YOUR APP ID#> with the app ID in the dashboard.
4. Open app/build.gradle and add the following line to the dependencies list:
      ...
      dependencies {
          ...
          compile 'io.agora.rtc:full-sdk:2.1.0' 
      }
5. Run the sample application in Android Studio. Move the first device until you find a horizontal surface.
6. Touch the plane indicator to add a virtual display screen to your AR session. The virtual display screen streams the video from the remote user.
7. On the second device, launch the Agent-AR_Chat sample application using the same app ID used in this project, and join the channel arcore as a broadcaster.
