set (public_docs osl-languagespec.pdf)
# Some day: CLA-INDIVIDUAL CLA-CORPORATE

install (FILES ${public_docs} DESTINATION ${CMAKE_INSTALL_PREFIX}/share/openshadinglanguage COMPONENT documentation)

install ( FILES ${PROJECT_SOURCE_DIR}/../LICENSE
                ${PROJECT_SOURCE_DIR}/../INSTALL
                ${PROJECT_SOURCE_DIR}/../CHANGES
                ${PROJECT_SOURCE_DIR}/../README.md
          DESTINATION ${CMAKE_INSTALL_PREFIX}/share/openshadinglanguage )

