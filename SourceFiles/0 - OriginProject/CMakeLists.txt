cmake_minimum_required(VERSION 3.1)

set(CMAKE_CXX_STANDARD 11)

# set Qt moc rcc uic
set(CMAKE_AUTOMOC ON)
set(CMAKE_AUTORCC ON)
set(CMAKE_AUTOUIC ON)

project(Feimos)

set(CMAKE_BUILD_TYPE  "Debug")

set(QT_PATH "D:/DevTools/QT5/5.7/msvc2015_64" CACHE PATH "qt5 cmake dir")

set(CMAKE_PREFIX_PATH ${QT_PATH})

find_package(Qt5 COMPONENTS 
	Widgets 
	Gui 
REQUIRED)

# include files
INCLUDE_DIRECTORIES(
	${QT_INCLUDE_DIR}
	${CMAKE_CURRENT_BINARY_DIR}
	${CMAKE_CURRENT_SOURCE_DIR}
)

# Main GUI files
set(MainGUI
	MainGUI/main.cpp
	MainGUI/MainWindow.h
	MainGUI/mainWindow.cpp
	MainGUI/DebugText.hpp
	MainGUI/DebugText.cpp
	MainGUI/DisplayWidget.h
	MainGUI/DisplayWidget.cpp
	MainGUI/IMAGraphicsView.h
	MainGUI/IMAGraphicsView.cpp
	MainGUI/RenderThread.h
	MainGUI/RenderThread.cpp
	MainGUI/InteractionDockWidget.h
	MainGUI/InteractionDockWidget.cpp
)
# Make the MainGUI group
SOURCE_GROUP("MainGUI" FILES ${MainGUI})

# Core files
set(Core
	# 数据存储
	Core/FrameBuffer.h
	Core/FrameBuffer.cpp
)
# Make the Core group
SOURCE_GROUP("Core" FILES ${Core})

# Create executable
add_executable(Feimos
	WIN32
	${MainGUI}
	${Core}
)

FILE(GLOB Icons ${CMAKE_CURRENT_SOURCE_DIR}/Icons/*.png)
SET(EXECUTABLE_OUTPUT_PATH ${CMAKE_CURRENT_BINARY_DIR})
file(COPY ${Icons} DESTINATION ${EXECUTABLE_OUTPUT_PATH}/Icons/)

target_link_libraries(Feimos 
	Qt5::Widgets
	Qt5::Gui
)

set_property(DIRECTORY ${CMAKE_CURRENT_SOURCE_DIR} PROPERTY VS_STARTUP_PROJECT Feimos)




