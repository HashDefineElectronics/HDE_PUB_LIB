# HDE_PUB_LIB
Hash Define Electronics Public Kicad Library

#### Instructions
- Clone `git@github.com:HashDefineElectronics/HDE_PUB_LIB.git` next to your KiCad project directory and not inside it.
- Add the *.lib files found in the Libary folder to your KiCad eeschema libraries setting.
- You will need to use `${KIPRJMOD}/../HDE_PUB_LIB/Footprint/` when adding the individual footprint to your project libary. (Note: `${KIPRJMOD}` is internal set by KiCad to the current project root directory)
- Or use the *fp-lib-table* example bellow.

#### fp_lib_table example
This is what the fp_lib_table would look like if HDE_PUB_LIB is the only footprint library used in the project.
```
(fp_lib_table
  (lib (name Capacitors)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Capacitors.pretty)(options "")(descr ""))
  (lib (name Connectors)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Connectors.pretty)(options "")(descr ""))
  (lib (name Crystals)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Crystals.pretty)(options "")(descr ""))
  (lib (name Diodes)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Diodes.pretty)(options "")(descr ""))
  (lib (name Fuses)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Fuses.pretty)(options "")(descr ""))
  (lib (name HDE)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/HDE.pretty)(options "")(descr ""))
  (lib (name IC)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/IC.pretty)(options "")(descr ""))
  (lib (name Inductor)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Inductor.pretty)(options "")(descr ""))
  (lib (name Miscellaneous)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Miscellaneous.pretty)(options "")(descr ""))
  (lib (name Modules)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Modules.pretty)(options "")(descr ""))
  (lib (name Mount)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Mount.pretty)(options "")(descr ""))
  (lib (name Resistors)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Resistors.pretty)(options "")(descr ""))
  (lib (name Switches)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Switches.pretty)(options "")(descr ""))
  (lib (name Via)(type KiCad)(uri ${KIPRJMOD}/../HDE_PUB_LIB/Footprint/Via.pretty)(options "")(descr ""))
)
```
