# How to build Gen 9 Shaders.

#### ***This is Experimental and not completely working***

### Requirements:
 - A prebuilt version of normal shaders, you can compile them or download them
 - Make sure you setup the source code (follow all steps on PC Guide up to [Patching Source Code and Tools](https://github.com/FranklinClintonDev/gta-v-source-code-guide/blob/main/PC.md#patching-source-code-and-tools)

### Compile Shaders
1. Launch `X:\gta5\src\dev_ng\game\VS_Project\load_sln_unity_2012.bat\load_sln_unity_2012` to load up the solution and wait for it to load. 
2. Make sure your platform is on `x64`.
3. On your solution explorer scroll down to `shaders_rc` and right click on properties 
4. Double check that your platform is `Win32` and your configuration is `(Debug Win32 4.0)`

# PROGRESS MARK (After this the info is not tested by me)

5) Rename this
`$(MSBuildProjectDirectory)\batch\rsm_build_win32_40.bat dev`
`$(MSBuildProjectDirectory)\batch\rsm_rebuild_win32_40.bat dev`
`$(MSBuildProjectDirectory)\batch\rsm_clean_win32_40.bat dev`

To this 
`$(MSBuildProjectDirectory)\batch\rsm_build_win32_50.bat dev`
`$(MSBuildProjectDirectory)\batch\rsm_rebuild_win32_50.bat dev`
`$(MSBuildProjectDirectory)\batch\rsm_clean_win32_50.bat dev`

6. After that build the shaders with incredibuild.
7. Wait for the build to finish (Expect for errors and the build to fail)
8. After the build finshes 90% of the build should have stil completed
9. Your compiled sharders should be `X:\gta5\titleupdate\dev_ng\common\shaders`
10. Drag the contents from `win32_50` to `win32_40` in your shaders folder
11. Launch the build and enjoy!
