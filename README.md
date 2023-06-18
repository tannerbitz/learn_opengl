### PURPOSE
This repo is a playground to learn OpenGL.  As of this first writing, it follows along the OpenGL series from TheCherno on YouTube


### SETUP
#### Install Conan Package Manager
```
python3 -m pip install conan
conan profile detect
```

### BUILDING
```
conan build -b missing .
```

Note: As of this writing, this transitively depends on the conan package `opengl/system`. This uses your system package manager to download packages and thus may require the following conan config settings. You may need to add these your build profile:

```
[conf]
tools.system.package_manager:mode=install
tools.system.package_manager:sudo=True
```