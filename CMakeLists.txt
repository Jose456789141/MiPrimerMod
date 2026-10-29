cmake_minimum_required(VERSION 3.13)
include(FetchContent)

FetchContent_Declare(
    Geode
    GIT_REPOSITORY https://github.com/geode-sdk/geode
    GIT_TAG v2.0.0
)
FetchContent_MakeAvailable(Geode)

project(MiPrimerMod VERSION 1.0.0 LANGUAGES CXX)

setup_geode_mod(
    NAME MiPrimerMod
    ID tu-usuario.mi-primer-mod
)

add_subdirectory(src)
