## Installing SFML

1. **Download SFML:** Obtain the SFML library from the official website. Save the SFML folder to your `C:\` drive.

2. **Edit the PATH variable:**
    - Search Environment Variables in Windows. Click Environment Variables
    - In the Environment Variables window, locate the "Path" variable under the Systems Variable section and click "Edit."
    - Add the path "C:\SFML\bin" to the end of the system path variable, ensuring to separate directories with a semi-colon (`;`).

3. **Create SFML_SDK Environment Variable:**
    - In the Environment Variables window, click "New" under the "User variables" section.
    - Enter `SFML_SDK` as the Variable name and set its value to the SFML directory path, for example, "C:\SFML\".

## Building a Visual Studio project to use SFML

1. **Project Configuration:**
    - Open your Visual Studio project.

2. **Configure Include Directories:**
    - Go to project properties and select "All Configurations."
    - Under C/C++ -> General, add "$(SFML_SDK)\include" to the list of include directories.

3. **Configure Library Directories:**
    - Still in project properties, under Linker -> General, add "$(SFML_SDK)\lib" to the list of library directories.

4. **Additional Configuration:**
    - Make sure your project settings are correctly set up to link against SFML libraries during compilation and linking processes.
    - Don't forget to click "Apply" when you have added the links to the additional libraries and includes.
