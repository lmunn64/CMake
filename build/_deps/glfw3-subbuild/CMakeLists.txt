# Distributed under the OSI-approved BSD 3-Clause License.  See accompanying
# file Copyright.txt or https://cmake.org/licensing for details.

cmake_minimum_required(VERSION 3.22.1)

# We name the project and the target for the ExternalProject_Add() call
# to something that will highlight to the user what we are working on if
# something goes wrong and an error message is produced.

project(glfw3-populate NONE)



include(ExternalProject)
ExternalProject_Add(glfw3-populate
                     "UPDATE_DISCONNECTED" "False" "FIND_PACKAGES_ARGS" "3.4" "URL" "https://github.com/glfw/glfw/archive/refs/tags/3.4.tar.gz"
                    SOURCE_DIR          "/mnt/d/Desktop/Projects/game/build/_deps/glfw3-src"
                    BINARY_DIR          "/mnt/d/Desktop/Projects/game/build/_deps/glfw3-build"
                    CONFIGURE_COMMAND   ""
                    BUILD_COMMAND       ""
                    INSTALL_COMMAND     ""
                    TEST_COMMAND        ""
                    USES_TERMINAL_DOWNLOAD  YES
                    USES_TERMINAL_UPDATE    YES
)


