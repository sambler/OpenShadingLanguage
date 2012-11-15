SET ( oslinfo_srcs oslinfo.cpp )
ADD_EXECUTABLE ( oslinfo ${oslinfo_srcs} )
LINK_ILMBASE ( oslinfo )
TARGET_LINK_LIBRARIES ( oslinfo oslquery ${OPENIMAGEIO_LIBRARY} ${Boost_LIBRARIES} ${CMAKE_DL_LIBS})
INSTALL ( TARGETS oslinfo RUNTIME DESTINATION bin )

if (WIN32 AND BUILDSTATIC)
    TARGET_LINK_LIBRARIES ( oslinfo psapi.lib )
endif ()
