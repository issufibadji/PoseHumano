## PoseHumano
# A.Requisitos: 
1. OpenCV > 3.4.1
2. excute getModels.sh na linha de comando Ou faça o download do modelo caffe de http://posefs1.perception.cs.cmu.edu/Users/ZheCao/pose_iter_440000.caffemodel e colocá-lo coco folder

# B. Para usar a C++ (Compilando o arquivo cpp)
 
Usa g++
Comando para compilar o arquivo cpp no ​​Ubuntu:
  1-cria uma arquivo Makefile
  2-copia e cola a configuração abaixo:
  ""
    TARGET=a.out
    CXX=g++
    LD=g++
    OPENCV=-I/usr/include/opencv4 -g
    #CXXFLAGS=-lopencv_core -lopencv_imgproc -lopencv_highgui -lopencv_imgcodecs -lopencv_objdetect -lopencv_features2d -std=c++11
    CXXFLAGS=`pkg-config --cflags --libs opencv4`
    all:
      $(CXX) $(OPENCV) main.cpp $(CXXFLAGS)
      @./$(TARGET)
  ""
  3-excute :
  $ make
  $ ./a.out


# C. Para Codigo Python
 excute: 
 $ python main.py
