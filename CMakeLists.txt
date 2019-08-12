
cmake_minimum_required (VERSION 3.0)

if (TOOL)

    project (Tool VERSION 1.0.0 LANGUAGES CXX)

    add_subdirectory (util)

    add_subdirectory (tool)

elseif (APP)

    project (App VERSION 1.0.0 LANGUAGES CXX)

    add_subdirectory (util)

    add_subdirectory (app)

else ()

    project (Root VERSION 1.0.0 LANGUAGES CXX)

    add_subdirectory (util)

    add_subdirectory (tool)

    add_subdirectory (app)

endif ()
