# docker-enclose
[![](https://badge.imagelayers.io/coopermaa/enclose:latest.svg)](https://imagelayers.io/?images=coopermaa/enclose:latest 'Get your own badge on imagelayers.io')

Docker image for [encloseJS](http://enclosejs.com/)

## How to use this image

Convert a Node.js program into a stand-alone executable:

```bash
# Create a hello.js
$ echo 'console.log("Hello Node.js");' > hello.js

# Convert hello.js into a stand-alone executable result in an ELF executable as './hello'
$ docker run -v $(pwd):/code coopermaa/enclose --x64 -o hello hello.js

# Run the executable
$ ./hello
Hello Node.js
```