
if (CONFIG_MCUX_COMPONENT_middleware.libjpeg)
    mcux_add_source(
        SOURCES inc/cderror.h
                inc/cdjpeg.h
                inc/jdct.h
                inc/jerror.h
                inc/jinclude.h
                inc/jmemsys.h
                inc/jmorecfg.h
                inc/jpegint.h
                inc/jpeglib.h
                inc/jversion.h
                inc/transupp.h
                src/jaricom.c
                src/jcapimin.c
                src/jcapistd.c
                src/jcarith.c
                src/jccoefct.c
                src/jccolor.c
                src/jcdctmgr.c
                src/jchuff.c
                src/jcinit.c
                src/jcmainct.c
                src/jcmarker.c
                src/jcmaster.c
                src/jcomapi.c
                src/jcparam.c
                src/jcprepct.c
                src/jcsample.c
                src/jctrans.c
                src/jdapimin.c
                src/jdapistd.c
                src/jdarith.c
                src/jdatadst.c
                src/jdatasrc.c
                src/jdcoefct.c
                src/jdcolor.c
                src/jddctmgr.c
                src/jdhuff.c
                src/jdinput.c
                src/jdmainct.c
                src/jdmarker.c
                src/jdmaster.c
                src/jdmerge.c
                src/jdpostct.c
                src/jdsample.c
                src/jdtrans.c
                src/jerror.c
                src/jfdctflt.c
                src/jfdctfst.c
                src/jfdctint.c
                src/jidctflt.c
                src/jidctfst.c
                src/jidctint.c
                src/jmemmgr.c
                src/jmemnobs.c
                src/jquant1.c
                src/jquant2.c
                src/jutils.c
    )
    mcux_add_include(
        INCLUDES inc
    )
endif()

if (CONFIG_MCUX_COMPONENT_middleware.libjpeg.template)
    mcux_add_source(
        SOURCES template/jconfig.h
        CONFIG true
    )
    mcux_add_include(
        INCLUDES template
        TARGET_FILES jconfig.h
    )
endif()
