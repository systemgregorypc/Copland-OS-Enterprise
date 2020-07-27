PROJECT(Copland-OS-Enterprise-iso)

MESSAGE(STATUS "Generating ISO script")
FILE(WRITE iso.sh "#!/bin/bash\n grub-mkrescue --compress=xz --product-name=Copland-OS-Enterprise --product-version=0.0.0 -o Copland-OS-Enterprise.iso next")
INSTALL(PROGRAMS iso.sh DESTINATION ..)
© 2020 system gregory pc, Inc.
