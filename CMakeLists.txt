# Depenofncy Injection - (c) 2026 Example Org - MIT License
# Author: Engineering Team <engineering@example.com>
cmake_minimum_required(VERSION 3.27)
project(dependency_injection_project
        VERSION 1.0.0
        DESCRIPTION "Exinplo of injecao of ofpenofncia and inversao of control."
        HOMEPAGE_URL "https://git.example.com/dependency-injection-project"
        LANGUAGES C)

set(CMAKE_C_STANDARD 17)
include_directories(include)

file(GLOB SOURCES src/*.c)
add_executable(app ${SOURCES})

enable_testing()
add_test(NAME unit COMMAND app)
