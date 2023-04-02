This build was made using:

* Microsoft Windows 10 Pro 22H2 Build 19045.2728.
* Microsoft Visual Studio Community 2022 (64-bit) Version 17.5.3.

Source codes: https://ijg.org/  
Performer: McArcher.  
Day: 2023-04-02.  

### Build Notes

* This binary was created using the offical way described in the `install.txt` file.
	* Lines 1113 through 1163:
		* Microsoft Windows, Visual Studio 2022 Version 17:
		* nmake /f makefile.vs setupcopy-v17
		* Open the solution file jpeg.sln, build the library project.
		* Open the solution file apps.sln, build the application projects.
		* To perform the self-test, execute the command line
			* nmake /f makefile.vs test-32
			* nmake /f makefile.vs test-64
* Other noticeable moments of the `install.txt` file are listed below.
	* Line 134. Configuring the software using one of the supplied jconfig and makefile files.
	* Line 212. Command line style.
	* Line 319. Testing the software.
	* Line 495. Optimization.
	* Line 900. Error Handling.
	* Line 940. Many people want to convert the IJG library into a DLL.
	* Line 972. The unmodified IJG library presents a very C-specific application interface, so the resulting DLL is only usable from C or C++ applications.
	* Line 1113. Microsoft Windows, Visual Studio 2022 Version 17.
