=============================================
           RISCV-32I IMPLEMENTATION
=============================================
A C++ Implementation of RISCV-32I Processor

---------------------------------------------
                  README
---------------------------------------------

TABLE OF CONTENTS:
1. Developer Details
2. Directory Structure
3. How to Build
4. How to Execute
5. How to View Output/GUI

---------------------------------------------
            DEVELOPER DETAILS
---------------------------------------------

👨‍💻 Developer: **Girish Kumar**
🔢 Entry Number: 2022csb1083
📧 Email: 2022csb1083@iitrpr.ac.in

👨‍💻 Developer: **Devraj Behl**
🔢 Entry Number: 2022csb1077
📧 Email: 2022csb1077@iitrpr.ac.in

👨‍💻 Developer: **Shashank Kumar**
🔢 Entry Number: 2021csb1131
📧 Email: 2021csb1131@iitrpr.ac.in

---------------------------------------------
           DIRECTORY STRUCTURE
---------------------------------------------
```
RISCV-32I-Implementation
  ├── bin
  │   ├── RISCV
  │   ├── Data Memory.mc
  ├── doc
  │   ├── Design Doc.docx
  ├── include
  │   ├── Core.h
  │   ├── CacheFile.h
  │   ├── GUI.h
  │   ├── Pipeline.h
  │   ├── RISCV.h
  ├── src
  │   ├── Core.cpp
  │   ├── CacheFile.cpp
  │   ├── GUI.cpp
  │   ├── Pipeline.cpp
  │   ├── main.cpp
  │   ├── Makefile
  │   ├── RISCV.cpp
  ├── test
  │   ├── bubblesort.s
  │   ├── bubblesort.mc
  │   ├── fibonacci.s
  │   ├── fibonacci.mc
  ├── gui
  │   ├── public
  │   │   ├── index.html
  │   │   ├── styles.css
  │   ├── src
  │   │   ├── App.jsx
  │   │   ├── index.js
  │   │   ├── components
  │   │   │   ├── filedata.json
```
---------------------------------------------
              HOW TO BUILD
---------------------------------------------
📌 **Compiling:**
```sh
$ cd src
$ make
```
📌 **Cleaning the project:**
```sh
$ cd src
$ make clean
```
---------------------------------------------
             HOW TO EXECUTE
---------------------------------------------
📌 **Command to execute program:**
```sh
../bin/RISCV <knobs>
```
📌 **Knobs Usage:**
```
-test <filename.mc> (Compulsory)
-n <value of N>
-pipeline
-forward
-trace [<instruction number>]
-registers
-h or -help
```
ℹ️ **Additional Info:**
- `-h` or `-help` shows execution details
- Default value of `N` is 5
- Pipelining, forwarding, tracing, and register display are OFF by default
- `forward/trace` require `pipeline` to be enabled
- `-trace <instruction>` traces a specific instruction; otherwise, all
- `-registers` displays register values after each cycle

---------------------------------------------
          HOW TO VIEW OUTPUT/GUI
---------------------------------------------
📌 **Data Memory Storage:**
```
../bin/Data Memory.mc
```
📌 **Run the following commands to view GUI:**
```sh
$ cd ../gui
$ npm i react-scripts
$ npm start
```

