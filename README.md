Darwin ARM SDK
==============

NOTE: This is a preliminary release, things are subject to change without notice!

This SDK depends on the following packages to be installed on your system:

	* llvm (>=3.2)
	* libuuid1
	* uuid-runtime
	* libssl
	* libblocksruntime
	* flex
	* tcsh
	* bison
	* make
	* unifdef
	* autotools-dev

What is What is included in this SDK:

	* Developer tools:
		- image3maker		- a simple utility used to generate img3 files to be used when building GenericBooter
		- developer_cmds	- a port of apple's open source developer tools
		- bootstrap_cmds	- a port of the Mach Interface Generator

	* Toolchain tools:
		- clang/llvm		- a slightly modified port of clang-3.4 that is used to cross compile code for Darwin ARM. Also includes other llvm tools
		- cctools		- a port of apple's other misc. compiler tools

	* System tools:
		- xcode-tools		- tools used to invoke Darwin ARM sdk tools or get Toolchain/SDK information from anywhere on your system
					 NOTE: you should invoke all SDK commands through xcrun. see https://github.com/b-man/xcode-tools.git for more info

	* Developer resources:
		- CoreOSMAkefiles	- for compatibility purposes (Don't use this directly!)
		- avaliability		- used for library versioning
		- Darwin ARM sysroot	- the Darwin ARM sysroot - contains all necessary userspace headers/libraries (based on iOS5.x sdk sysroot)


How to install this SDK:

	* for now, this SDK is only available in tar.bz2 form. To install this SDK into your system, run the following as root:

		```
		tar -jxpf DarwinARM_SDK_v0.1_32bit.tar.bz2
		mv -f DarwinARM_SDK_v0.1_32bit/* /
		```
