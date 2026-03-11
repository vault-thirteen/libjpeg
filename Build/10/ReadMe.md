This build was made using:

* Microsoft Windows 10 Pro 22H2 Build 19045.7058.
* Microsoft Visual Studio Community 2022 (64-bit) Version 17.14.28.

Source codes: https://ijg.org/  
Performer: McArcher.  
Day: 2026-03-11.  

### Build Notes

* This binary was created using the official way described in the `install.txt` file.
	* Lines 1065 through 1119:
		* Microsoft Windows, Microsoft Visual Studio 2019-2026 version 16-18:
		* `nmake /f makefile.vs setupcopy-v16`
        * Open the solution file `jpeg.sln`, build the library project.
        * Open the solution file `apps.sln`, build the application projects.
		* To perform the self-test, execute the command line
			* `nmake /f makefile.vs test-32`
			* `nmake /f makefile.vs test-64`
* Other noticeable moments of the `install.txt` file are listed below.
	* Line 134. Configuring the software using one of the supplied jconfig and makefile files.
	* Line 217. Command line style.
	* Line 324. Testing the software.
	* Line 500. Optimization.
	* Line 896. Error Handling.
	* Line 945. Many people want to convert the IJG library into a DLL.
	* Line 977. The unmodified IJG library presents a very C-specific application interface, so the resulting DLL is only usable from C or C++ applications.
	* Line 1064. Microsoft Windows, Microsoft Visual Studio 2019-2026 version 16-18.

## Integrity Meta Data

Integrity can be verified using following parameters:
* File sizes
	* See the `file_sizes.txt` file, [Link](./file_sizes.txt).


* CRC32 check sums
	* See the `crc32_sums.txt` file, [Link](./crc32_sums.txt).


* SHA-256 check sums
	* See the `sha256_sums.txt` file, [Link](./sha256_sums.txt).

**Notes**

Checks of hash sums & sizes can be performed with a `Hasher` tool.  
Hasher's repository: https://github.com/vault-thirteen/Hasher
