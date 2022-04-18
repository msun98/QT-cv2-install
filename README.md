# QT-cv2-install

INCLUDEPATH += C:\Users\rainbow\Documents\common\opencv-msvc\build\include
INCLUDEPATH += "C:\Program Files (x86)\Intel RealSense SDK 2.0\include" # 리얼센스 sdk 인클루드 폴더(절대경로)


# 오픈시브이용 디버그 모드이면 opencv_world455d 파일 실행. 릴리즈 모드이면 opencv_world455 파일 실행.
CONFIG(debug, debug|release):LIBS += C:\Users\rainbow\Documents\common\opencv-msvc\build\x64\vc15\lib\opencv_world455d.lib //디버그 모드일 때 실행
CONFIG(release, debug|release):LIBS += C:\Users\rainbow\Documents\common\opencv-msvc\build\x64\vc15\lib\opencv_world455.lib //릴리즈 모드일 때 실행

# 리얼센스용
CONFIG(debug, debug|release):LIBS += "C:\Program Files (x86)\Intel RealSense SDK 2.0\lib\x64\realsense2.lib"
CONFIG(release, debug|release):LIBS += "C:\Program Files (x86)\Intel RealSense SDK 2.0\lib\x64\realsense2.lib"
