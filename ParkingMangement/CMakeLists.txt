cmake_minimum_required(VERSION 3.0.0)
set(PROJECT_NAME parkingmangement)
set(SRC_LIST main.c simpleMenu.c menuAction.c parkingLot.c linkStack.c seqQueue.c seqStack.c debug.c)
project(${PROJECT_NAME})
add_executable(${PROJECT_NAME} ${SRC_LIST})