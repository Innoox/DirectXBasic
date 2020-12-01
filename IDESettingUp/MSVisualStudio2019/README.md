# Setting-Up Microsoft Visual Studio 2019 for the work with DirectX 11

1. Create an empty project
2. Right click on the project name and select **Properties**
3. Under the **Configuration Properties** in the:
	- **General** tab change _C++ Language Standard_ to the **ISO C++ 17**
	- **Advanced** tab:
		1. change _Use of MFC_ to the **Use MFC in a Static Library**
		2. change _Character Set_ to the **Use Multi-Byte Character Set**
4. Under the **C/C++** in the:
	- **General** tab change _Warning Level_ to the **Level2 (/W2)**
	- **Optimization** tab change _Optimization_ to the **Disabled(/Od)**
	- **Preprocessor** tab change _Preprocessor Definitions_ to the **_DEBUG;_MODE;**
	- **Precompiled Headers** change to the **Not Using Precompiled Headers**
5. Under the **Linker** in the
	- **Input** tab  add to _Additional Dependecies_:
		1. d3d11.lib