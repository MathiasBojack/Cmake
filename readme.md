# Command

- The *project* command, ex:
```sh
    project("HelloWorld")
```
- gives the project a name
- gives a couple of variables, such as the *PROJECT_NAME* variable


- *Dereference* a variable to get the value of the variable:
```sh
    ${variableName}
    "${stringVariableName}"
```

A good practice for dereferencing a string variable is to put the variable in between double quotes. CMake use spaces as delimiter, if strings are not put double quotes, you may have a parsing error.

- *add_executable* command
create an executable targets in CMake

```sh
add_executable("nameOfTheExecutable" "sourceCodeToBuildTheExecutable")

- *install* command

```sh
install(TARGETS "targetName" DESTINATION desDirectory)
```

Here the desDirectory is the path relative to the CMake install prefix, namely, ${CMAKE_INSTALL_PREFIX}/desDirectory

# CMake Gui

- CMake accepts two paths: 
    - Top path should point to top level CMakeLists.txt file
    - Second path point to the build directory
- After finishing configuration, CMake cash variables will be populated in the window. CMake cash variables are used to customize the build.

![CMake](./ex1/fig/CMake.png)