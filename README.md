# Zygisk Module Template

An Zygisk Module Template based on zygisk-module-sample. Both cmake and ndk-build are supported.

## Usage

1. Edit your moduleId in [build.gradle.kts](./build.gradle.kts) (It's also your module's soname).  
2. Edit other module info in build.gradle.kts or module/template/module.prop.  
3. Write your code in module/src/main/cpp .  
4. Run gradle task `:zipDebug` or `:zipRelease` to build the module. 
   Your module zip will be generated under `module/release`. 
5. Run gradle task `:install(Magisk|Ksu)[AndReboot](Debug|Release)` to flash your module (optional).  

## See also

https://github.com/topjohnwu/zygisk-module-sample
