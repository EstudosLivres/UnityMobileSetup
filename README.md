# UnityMobileSetup
Setup Unity for mobile development with XCode iOS simulator tests

## Summary/CheckList

- [ ] [LWRP (2019 or lower versions) or Universal Pipeline (2020 unity version)](#lwrp)
- [ ] [Switch Platform (iOS on MAC)](#summarychecklist)
- [ ] [Define orientation only (portrait or landscape)](#define-orientation)
- [ ] [iOS Processing](#ios-processing)

# LWRP

1. Menu bar at Unity:
    1. Window > Package Manager
      1. All Packages (filter)
          1. Lightweight RP > Install
          
          ![LWRPInstall](https://user-images.githubusercontent.com/3121488/69914293-502faf00-1421-11ea-9968-a23e124b88df.png)
          
          1. LWRP Create
          
          ![LWRPCreate](https://user-images.githubusercontent.com/3121488/69914417-ed3f1780-1422-11ea-812d-76eccdd6da7f.png)
          
          1. LWRP Config
          
          ![LWRPConfig](https://user-images.githubusercontent.com/3121488/69914438-24adc400-1423-11ea-89be-6e13ee3c7c54.png)

          1. MenuBar > Edit > Project Settings > Graphics > Drag&Drop created LWRP (LWRP Set)
          
          ![LWRPSet](https://user-images.githubusercontent.com/3121488/69914473-b9182680-1423-11ea-8909-9587be8c5b75.png)
          
          1. after LWRP Set everything get pink (LWRP Process):
              
              1. MenuBar > Edit > Render Pipeline > Upgrade Project Materials to Render Pipeline
              
              ![LWRP Process](https://user-images.githubusercontent.com/3121488/69914575-a18d6d80-1424-11ea-841c-89e3ea135e8a.png)
              
              1. IF Still anything pink (update it specific shader):
              
              ![LWRP Specific Pink Process](https://user-images.githubusercontent.com/3121488/69915424-70fe0180-142d-11ea-9258-440606d8fc09.png)



# Switch Platform (prefer iOS on MAC)

1. Menu bar at Unity
    1. File
    1. Build Settings
        1. Select "iOS" and click on "switch platform"
        1. Click "Add Open Scenes"
1. Click "Player Settings" for the next steps

![Switch Platform](https://user-images.githubusercontent.com/3121488/69901430-3712f980-1360-11ea-8ac2-2888c34bf4b0.png)

# Define Orientation
At "Player Settings":
1. Select the platorm (phone icon is iOS)
  1. "Resolution and Presentation":
      1. Default Orientation = '>' (landscape) '^' (portrait)
  1. Allowed Orientations for Auto Rotation

![Define Orientation](https://user-images.githubusercontent.com/3121488/69913873-3f306f00-141c-11ea-81aa-449124183ad0.png)

# iOS Processing
1. Color Space = "Gamma"
1. Auto Graphic API = "Metal + OpenGLES3"
1. Bundle Identifier = "com.Company.Proj"
1. Target SDK = "Simulator SDK" (development) and "Device SDK" (production)
