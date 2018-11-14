### ANPR System: The Russian system of automatic number plate recognition

####Dependencies
* OpenCV >= 2.4.9
* leptonica >= 1.71
* Tesseract OCR >= 3.02

####Build (Ubuntu)
* Build dependencies

```
sudo apt-get update
sudo apt-get install build-essential git pkg-config
sudo libleptonica-dev libopencv-dev libopencv-contrib-dev libopencv-imgcodecs-dev libopencv-ml-dev libtesseract-dev libtesseract4
```

* Get the last build

```
git clone https://github.com/hardkun/Russian_System_of_ANPR.git
```

* Build the app

```
cd src
make
```

* Run the app

```
sudo locale-gen ru_RU.UTF-8
export TESSDATA_PREFIX="<projectdir>/runtime_data/tessdata"
cd runtime_data #xml data files have to be in binary execution directory
../src/rusalpr image.{jpg,png}
```


####Screenshots

![Gittip](http://i.imgur.com/3WfcwvR.png)
![Gittip](http://i.imgur.com/jCFUDqF.png)
![Gittip](http://i.imgur.com/7MloYGh.png)
![Gittip](http://i.imgur.com/qgbpOto.png)
![Gittip](http://i.imgur.com/1XiqEo3.png)
![Gittip](http://i.imgur.com/Uv8E4IA.png)
