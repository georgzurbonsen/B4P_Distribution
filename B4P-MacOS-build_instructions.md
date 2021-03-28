# Beyond4P_Distribution
Explore powerful language for processing large tables and big tables


# Building for MACOS
This uses the B4P sources for Linux, and builds for MacOS

__Requirements__
1. Beyond4P_Code  (git pull; copy to cpp folder)
2. Beyond4P_Installation_Linux (git pull; copy to cpp folder)
3. Beyond4P License File.json (download; copy to cpp folder)


__Beyond4P_Code folder__: change 'stdafx.h' file: 
```text
#define _MACOS  -> define _MACOS
#define _UTF8   -> define _UTF8
```

__XCODE Application__
1. Create new Xcode project
2. Template: macOS
3. Application: Command line tool
4. Product name: b4p-macos
5. Language: C++
6. Build 'main.cpp' -> 'Hello, World!'
7. Delete 'main.cpp' (move to trash)
8. From Beyond4P_Code, copy all  *.cpp and *.h to XCODE 'b4p-macos' folder
9. Build (arrow)
10. In 'Products' folder, right click on 'b4p-macos' binary and Show in Finder
11. copy 'b4p-macos' binary to Beyond4p_Distribution folder


__Beyond4P_Distribution folder__:
1. unzip Beyond4P_Installation_LINUX_64bit -> Beyond4P_Intallation
2. move 'b4p-macos' binary to Beyond4P_Installation folder
3. copy '/Users/rafael/cpp/Beyond4P License File.json' to Beyond4P_Installation folder


__Beyond4P_Installation folder__:
1. delete Beyond4P binary
2. rename 'b4p-macos' to 'Beyond4P'
3. change permissions all all files and folders in Installation folder to 755


__Installation__
```text
> sudo ./setup
```

__Directory Settings__

```text
    For executable program:                     /usr/local/bin
    For program related files (libraries):      /usr/local/etc/Beyond4P
    For user application data:                  /Users/rafael/.config/Beyond4P

    Found following settings files:

    User   settings:   /Users/rafael/.config/Beyond4P/Beyond4P User Settings.json
    Locale settings:   /Users/rafael/.config/Beyond4P/Beyond4P Locale Settings.json
    License file   :   /Users/rafael/.config/Beyond4P/Beyond4P License File.json
```

__Testing__
```text
> ./Hello World.b4p
```




Notes:  https://guides.github.com/features/mastering-markdown/
