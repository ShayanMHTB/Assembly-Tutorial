# Assembly Language -- Tutorial  

Here I practice a programming in Assembly language. These are a collection of your typical beginner level programms and scripts people write in JAVA, Python and other programming languages when they start learning, with the twist, that they are written in assembly langauges.

## System Specifications  

### Hardware  

* Macbook Pro 14" 2021
* CPU: Apple Silicon M1
* Memory: 16GB
* Storage: 512GB

### Software  

* Operating System: Mac OSX Ventura  
* CommandLine Tools:  
	* xcode-select version 2396.  
	* as - Mac OS X Mach-O GNU-based assemblers:  
		* Apple clang version 14.0.0 (clang-1400.0.29.202)
		* Target: arm64-apple-darwin22.2.0
		* Thread model: posix
	* ld – linker:  
		* configured to support archs: armv6 armv7 armv7s arm64 arm64e arm64_32 i386 x86_64 x86_64h armv6m armv7k armv7m armv7em  
		* LTO support using: LLVM version 14.0.0, (clang-1400.0.29.202) (static support for 29, runtime is 29)  
		* TAPI support using: Apple TAPI version 14.0.0 (tapi-1400.0.11)  

---  

## Description:  

After installing the necessary software and writing your application, simply make sure `xcode-select`, `as` and `ld` are installed:  

```bash
# Ask for xcode-selct version
xcode-select -v

# Ask for assembly langauge version
as -v

# Ask for linker version
ld -v
```  

Then you can simply write your assemly program, compile it, then link it to your commanLineToll to be able to run it in Terminal.  

```bash
# ~/hello-world.asm

# Compiling the application
as hello-world.asm -o hello-world.o

# Linking the application
ld hello-world.o hello-world -lSystem /Library/Developer/CommandLineTools/SDKs/MacOSX.sdk/usr/lib

# Run the application
./hello-world
```  
