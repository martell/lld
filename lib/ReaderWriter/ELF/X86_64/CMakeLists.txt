add_llvm_library(lldX86_64ELFTarget
  X86_64LinkingContext.cpp
  X86_64TargetHandler.cpp
  X86_64RelocationHandler.cpp
  X86_64RelocationPass.cpp
  LINK_LIBS
    lldELF
    lldReaderWriter
    lldCore
    LLVMObject
    LLVMSupport
  )

include_directories(.)

add_subdirectory(ExampleSubTarget)
