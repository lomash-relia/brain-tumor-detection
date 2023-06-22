# Brain Tumor Detection

The project uses teachable machine to generate **tflite model** to classify the 4 categories related to brain tumor :

1. glioma_tumor
2. meningioma_tumor
3. pituitary_tumor
4. no_tumor


**Flutter** is used for the client-side interface. Dependencies used :

1. Camera
2. tflite

### 📝 Note: 
- The model is train on Teachable Machine which is not recommended professionally.
- Various factors such as camera quality, image noise, training parameters and much more decide the accuracy of the machine.
- Also packages such as tflite have not been updated since 2 years as of 22/06/23. Hence it is not a good practice to use it.
## Acknowledgements

 - [Brain Tumor Dataset by Sartaj Bhuvaji](https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri)
 - [Teachable Machine](https://teachablemachine.withgoogle.com/train/image)
## Run Locally

Clone the project

```bash
  git clone https://github.com/lomash-relia/brain-tumor-detection.git
```

Run pub get from .yaml file or use 

```bash
  flutter pub get
```

Make sure your device is connected for debugging and now you can run it

```
if you encounter any issues, check
C:\Users\{user}\AppData\Local\Pub\Cache\hosted\pub.dev\tflite-1.1.2\android
and open build.gradle file.
In the end of the file you will find dependencies 
where you should change "compile" to "implementation".
Save it and your project should run fine.
```