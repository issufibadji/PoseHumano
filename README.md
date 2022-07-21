<h1 align="center" color="yelow">
  PoseHumano
</h1>

<p align="center">
    <a href="#book-sobre">Sobre</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
    <a href="#rocket-tecnologias">Tecnologias</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
💻  <a href="#Pre-Requisitos:">Requisitos</a>&nbsp;&nbsp;&nbsp;|&nbsp;&nbsp;&nbsp;
    <a href="#memo-licença">Licença</a>
</p>

<p align="center">
   
 <img alt="GitHub language count" src="https://img.shields.io/github/languages/count/issufibadji/profileissufibadji?style=flat-square">

 <img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/issufibadji/profileissufibadji?style=flat-square">

 <img alt="GitHub last commit" src="https://img.shields.io/github/last-commit/issufibadji/profileissufibadji?style=flat-square">

 <img alt="GitHub" src="https://img.shields.io/github/license/issufibadji/profileissufibadji?style=flat-square">
</p>

   ![ezgif com-gif-maker](https://user-images.githubusercontent.com/45535344/180133435-f00b1ffc-f2da-4f6c-ac22-083ae4b2a270.gif)

## :book: Sobre

<!-- ❌✔️ -->
## :rocket: Tecnologias
Este projeto foi desenvolvido utilizando as seguintes tecnologias:
1. ✔️ Linguagem  C++
2. ✔️ Linguagem Python
3. ✔️ Biblioteca de Oponcv
 
## Pre-Requisitos: 
  ### Instalação das biblotecas
  1. ✔️ OpenCV > 3.4.1
  2. ✔️ excute getModels.sh na linha de comando Ou faça o download do modelo caffe de http://posefs1.perception.cs.cmu.edu/Users/ZheCao/pose_iter_440000.caffemodel e colocá-lo coco folder

### B. Para usar a C++ (Compilando o arquivo cpp)
 
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
 
 
