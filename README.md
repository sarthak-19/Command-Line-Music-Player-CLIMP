# Command Line Music Player CLIMP
 This is a mini project with C++ to create a command line based music player using MciSendStrings

**Sample Screenshots**

![1](https://user-images.githubusercontent.com/69689387/120195363-52eca980-c23c-11eb-86ec-e339c3741b21.JPG)

![2](https://user-images.githubusercontent.com/69689387/120195387-5aac4e00-c23c-11eb-82b6-263080cd5fea.JPG)

![3](https://user-images.githubusercontent.com/69689387/120195394-5d0ea800-c23c-11eb-92e2-4f7827c05a93.JPG)

![4](https://user-images.githubusercontent.com/69689387/120195402-5ed86b80-c23c-11eb-837e-bd570db55f73.JPG)

**Introduction:**

The Project to be developed is a Command Line Based Music Player completely written in C++.
It should play, pause and shuffle all music files in a specific directory and all it’s interface should be in C++ command line terminal.
We have divided the code into three files namely files.h , define.h , and main.cpp so as to improve code readability and debugging.

**Objective:**

The main objective is to play any non variable bit rate mp3 file using mciSendStrings() function defined in C++ windows.h header file.

**Instructions**

1. To run this code in visual studio code you have to add linker library -lwinmm here
![Linker](https://user-images.githubusercontent.com/69689387/120196237-3bfa8700-c23d-11eb-9bec-b4a102023be1.JPG)
It's a Windows Multimedia Library

2. If you are using code blocks or Visual Studio IDE you can directly add path of lwinmm in linker library options.
3. If you want to add more songs you can add it in songs folder after converting mp3 files to mono bitrate.

**Problem Faced :**

1. MciSendStrings documentation by Microsoft was very vague and lacked crucial informations like examples to demonstrate the working of its function.
2. MciSendStrings has 2 versions for its string command parameters. One accepts ANSI encoded characters while other accepts UNICODE and there was no proper information available regarding this.
3. To use MciSendStrings we need to link a library called -lwinmm (Windows Multimedia Lib) but there was no direct way to implement this Visual Studio Code as all the development work is done of Visual Studio IDE.
4. Windows Media Library provides very limited options in regards to the attributes of media file such as it could only play mono bit rate audio files with greatly reduced sample rate and hence offering poor sound quality.

We have also implemented error handling so that is any audio file could not be played for any reason the program will automatically skip to the next music in the list.


**Conclusion :**

There are many overheads to make a fully fledged music player via C++, but with the help of above code we have demonstrated a good example of how to make this work on C++ despite of having so many compatibility issues.

**Working Environment:**

1. Visual Studio Code - 1.56.2
2. C++ standard 17
3. Operating System – Windows 10 64 Bit
4. C++ Compiler – MinGW gcc x64

**References**

1. CodeProject -  https://www.codeproject.com/Articles/14709/Playing-MP3s-using-MCI
2. Stackoverflow - https://stackoverflow.com/questions/22253074/how-to-play-or-open-mp3-or-wav-sound-file-in-c-program
3. Codespeedy - https://www.codespeedy.com/play-a-part-of-an-mp3-file-in-cpp/
4. Github - https://github.com/microsoft/vscode-cpptools/issues/6191


