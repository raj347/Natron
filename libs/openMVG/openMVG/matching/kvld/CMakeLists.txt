
ADD_LIBRARY(openMVG_kvld kvld.cpp kvld.h algorithm.cpp algorithm.h)
SET_TARGET_PROPERTIES(openMVG_kvld PROPERTIES SOVERSION ${OPENMVG_VERSION_MAJOR} VERSION "${OPENMVG_VERSION_MAJOR}.${OPENMVG_VERSION_MINOR}")
SET_PROPERTY(TARGET openMVG_kvld PROPERTY FOLDER OpenMVG/OpenMVG)
INSTALL(TARGETS openMVG_kvld DESTINATION lib EXPORT openMVG-targets)
