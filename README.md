# Person_and_car_Detection_YOLOV5

<h3><b>System Setup for testing:</h3></b>
1) Install PyTorch as per your system requirement
Link: https://pytorch.org/ <br>
(GPU and CUDA is recommended for High FPS on Video, else for images its fine.)<br>
2) Create new Environment (pipenv or Conda)<br>
And install requirements.txt file using below command<br>
o pip install -r requirements.txt<br>
3) Incase you want to test this on YouTube videos, then install below 2 libraries additionally.<br>
o pip install youtube_dl<br>
o pip install pafy<br>
(System setup is ready and now your good to test)<br>

<h3><b>Testing:</b></h3>
<b>For images:</b> <br>
o python detect.py --source testimages/*.jpg --weights / best.pt<br>
<b>For YouTube Video: </b><br>
o python detect.py --source https://youtu.be/QIjZn_fiS3M --weights best.pt --conf <br>
0.25<br>
“--source” can be anything from below:<br>
◼ 0 # Webcam<br>
◼ file.jpg # image <br>
◼ file.mp4 # video<br>
◼ path/ # directory<br>
◼ path/*.jpg # glob<br>
◼ 'https://youtu.be/NUsoVlDFqZg' # YouTube video<br>
◼ 'rtsp://example.com/media.mp4' # RTSP, RTMP, HTTP stream<br>

“--weights”  by default, have I have kept best.pt <br>

<br><br>
![val_batch0_pred](https://user-images.githubusercontent.com/13836633/126869875-ba908b4b-96a9-449b-8582-31188483353c.jpg)

<br><br>
![val_batch1_pred](https://user-images.githubusercontent.com/13836633/126869878-88287525-a246-43c1-991e-3c8bd5ce40ce.jpg)

<br><br>
![val_batch2_pred](https://user-images.githubusercontent.com/13836633/126869881-ac9ed973-ea31-4cd9-acfc-274db3be0d36.jpg)
