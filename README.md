# Drowsiness-Detection

## Summary
In this project a drowsiness detector is implemented using YOLO. The training was performed with near infrared images. 
This project was developed in python programming language. 
The problem of drowsiness is something very common in people who perform activities such as surveillance, driving vehicles, among other activities  [^1]. Because of this, several algorithms based on artificial intelligence have been developed to detect drowsiness states.

![Imagen1](https://user-images.githubusercontent.com/44073142/173011408-ecbcee06-1166-45ac-af2c-0426c8440bb6.png)


## Problem Formulation
Drowsiness in drivers has been one of the main causes of traffic accidents [^2].
1.35 million deaths due to road accidents in 2016 worldwide [^3].
 
In Mexico, road accidents in 2015 were 378,232 [^4].

87% of road accidents are due to the driver [^2].

Studies from various countries show fatigue as responsible for between 20-30% of accidents occurring on highways [^2][^5].

## Near Infrared NIR
The near infrared (NIR) is a subset of the infrared band of the electromagnetic spectrum, covering wavelengths ranging from 0.7 to 1.4 microns. This wavelength is outside the range of what humans can see and sometimes provides clearer detail than can be achieved with visible light images [^6]. In the following figures we can see the electromagnetic spectrum as well as where the infrared band is located and the difference between a visible light image and a near infrared image.


![infra](https://user-images.githubusercontent.com/44073142/173011736-6c02e63a-cd34-414f-9c35-728eed309610.png)
![vis](https://user-images.githubusercontent.com/44073142/173007179-2b4288cf-1033-430d-9752-54362a09613d.png)

## Database Description
The selected infrared image database was Drozy Database with 700 near infrared images. 

![caras](https://user-images.githubusercontent.com/44073142/173008425-f4fe68d0-cc24-41c5-858d-a29bc1941533.png)

## Image labeling 
LabelImg software was used to label the images. Two classes were labeled, drowsiness and no-drowsiness.

![drow](https://user-images.githubusercontent.com/44073142/173008885-583591d8-0189-4227-a847-65815168c33d.png)
![no-drow](https://user-images.githubusercontent.com/44073142/173008924-89314005-2fef-44ca-b6bc-26c4eec0b67a.png)

## Training the model
The training is performed with 569 images. The time it takes is approximately 2 hours and 30 minutes. 

## Results
Once the training is completed, the network is tested with the test images. 

![drowsiness](https://user-images.githubusercontent.com/44073142/173009910-1b3d5b6e-949d-415c-8be1-fdd0bc67a424.png)
![no-drowsiness](https://user-images.githubusercontent.com/44073142/173010283-18f1d72b-301f-45d3-965b-3ea93efb08b6.png)

## Conclusions
The YOLO custom object detector allows us to train the network with our own images of what we want to detect, in this project we intended to detect drowsiness in near infrared images. A YOLOv4 detector was used, which was trained with over 500 images containing two classes, Drowsiness and No Drowsiness. Good results were obtained, however, they could be improved, because in some images the detector classifies in both classes at the same time. 

[^1]: M. PAEZ y E. ABARCA, “Herramientas para la seguridad en la movilidad, modelos predictivos de somnolencia en conductores”
[^2]: Chávez, L. G. (2018). La fatiga al conducir. Recuperado de: https://www.antp.org.mx/revista/86/articulo4.pdf.
[^3]: OMS (2016). Accidentes de tránsito 2015. 
[^4]: INEGI (2016). Síntesis metodológica de la estadística de accidentes de tránsito terrestre en zonas urbanas y suburbanas 2016. México: INEGI. 
[^5]: Chen, S., Wang, Z. y Chen, W. (2021). Driver drowsiness estimation based on factorized bilinear feature fusion and a long-short-term recurrent convolutional network. Information, 12(1), 3.
[^6]: T. Groenewald y H. Koster, “Espectroscopia de infrarrojo cercano (NIRS). La técnica de análisis rápidos del futuro”, Community of international Busines Related to Animal Production, 2006.




