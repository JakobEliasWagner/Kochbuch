cmake_minimum_required(VERSION 3.20 FATAL_ERROR)

project(
        Kochbuch
        VERSION 0.0
        DESCRIPTION "Eine Sammlung von Rezepten und Kalkulationstabellen"
        LANGUAGES NONE
)

set(PDFLATEX_COMPILER pdflatex)
set(LATEX_DEFAULT_BUILD pdf)

include(cmake/UseLATEX.cmake)

add_latex_document(main.tex)

