# HDE_PUB_LIB
Hash Define Electronics Public Kicad Library
## Adding Library

#### Method 1) Use the KiCad Template
Thanks to KiCad support for template projects, we can simple create a new project using the a premade template.

1. First clone the HDE_PUB_LIB anywhere in your system.
`git@github.com:HashDefineElectronics/HDE_PUB_LIB.git`
2. In KiCad create a new template project.
`File -> New project -> New project from tempalte`
3. Select the location where you want to create your project.
4. Then on the project template selector window, click on the `User templates`.
5. Click on the browse button and navigate to the `HDE_PUB_LIB/Template` and click OK.
6. Select the project and Click OK.
7. Now move HDE_PUB_LIB folder into your new KiCad Project.

The last step is important. The project is expecting the library to be located in the root directory of the project.


#### Method 2) Manually adding library to KiCad Project
the following instructions will go through the process of manually adding the HDE_PUB_LIB to an existing project.
- Clone `git@github.com:HashDefineElectronics/HDE_PUB_LIB.git` into the root directory of your project.
- Add the *.lib files found in the Library folder to your KiCad eeschema libraries setting.
- You will need to use `${KIPRJMOD}/HDE_PUB_LIB/Footprint/` when adding the individual footprint to your project library. (Note: `${KIPRJMOD}` is internal set by KiCad to the current project root directory)
- Or use the *fp-lib-table* example bellow.

#### fp_lib_table example
This is what the fp_lib_table would look like if HDE_PUB_LIB is the only footprint library used in the project.
```
(fp_lib_table
  (lib (name HDEP_Capacitors)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Capacitors.pretty)(options "")(descr ""))
  (lib (name HDEP_Connectors)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Connectors.pretty)(options "")(descr ""))
  (lib (name HDEP_Crystals)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Crystals.pretty)(options "")(descr ""))
  (lib (name HDEP_Diodes)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Diodes.pretty)(options "")(descr ""))
  (lib (name HDEP_Fuses)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Fuses.pretty)(options "")(descr ""))
  (lib (name HDEP_HDE)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_HDE.pretty)(options "")(descr ""))
  (lib (name HDEP_IC)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_IC.pretty)(options "")(descr ""))
  (lib (name HDEP_Inductor)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Inductor.pretty)(options "")(descr ""))
  (lib (name HDEP_Miscellaneous)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Miscellaneous.pretty)(options "")(descr ""))
  (lib (name HDEP_Modules)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Modules.pretty)(options "")(descr ""))
  (lib (name HDEP_Mount)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Mount.pretty)(options "")(descr ""))
  (lib (name HDEP_Resistors)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Resistors.pretty)(options "")(descr ""))
  (lib (name HDEP_Switches)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Switches.pretty)(options "")(descr ""))
  (lib (name HDEP_Via)(type KiCad)(uri ${KIPRJMOD}/HDE_PUB_LIB/Footprint/HDEP_Via.pretty)(options "")(descr ""))
)
```
