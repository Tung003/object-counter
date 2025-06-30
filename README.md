# Object Counting using Ultralytics YOLO11
use pretrained model YOLO11n detect and count the trucks

# Watch video

<p align="center">
  <a href="https://www.youtube.com/watch?v=NjB7Z-S0wT4">
    <img src="https://img.youtube.com/vi/NjB7Z-S0wT4/0.jpg" alt="Watch the video" />
  </a>
</p>

# 📊 Count trucks at border gates or BOT

Notebook: [📓 Xem tại đây](yolo.ipynb)

Or view with a nicer interface via 📘 [Mở notebook trên Colab (Google Drive)](https://colab.research.google.com/drive/16tjrC5jHRw7AiY6TwC7StqTqW0sK7NSN)

# Data

Cut 21 images from 3 video train 
<table align="center">
  <tr>
    <td align="center" width="45%">
      <img src="data_from_SAM2/data_from_SAM2/data/images/train/frame_train_28.jpg" width="100%"><br>
      <em>Image train</em>
    </td>
    <td align="center" width="45%">
      <img src="data_from_SAM2/data_from_SAM2/data/images/train/frame_train_196.jpg" width="100%"><br>
      <em>Image train</em>
    </td>
  </tr>
</table>


<table align="center">
  <tr>
    <td align="center" width="45%">
      <img src="data_from_SAM2/data_from_SAM2/data/images/train/frame_train3_28.jpg" width="100%"><br>
      <em>Image train</em>
    </td>
    <td align="center" width="45%">
      <img src="data_from_SAM2/data_from_SAM2/data/images/train/frame_train_56.jpg" width="100%"><br>
      <em>Image train</em>
    </td>
  </tr>
</table>

<p align="justify">
Use POLYGON ROBOFLOW get region points object in image 
Then SAM2 draws bounding box around the object and I will have x (x position), y (y position), w(width object), h(height object). with each image containing about 100 objects.
</p>
<table align="center">
  <tr>
    <td align="center" width="45%">
      <img src="img_detect_boundingbox_SAM2/img_detect_boundingbox_SAM2/result_SAM2_frame_train2_112.jpg" width="100%"><br>
      <em>SAM2</em>
    </td>
    <td align="center" width="45%">
      <img src="img_detect_boundingbox_SAM2/img_detect_boundingbox_SAM2/result_SAM2_frame_train_112.jpg" width="100%"><br>
      <em>SAM2</em>
    </td>
  </tr>
</table>

# Result train

</p>
<table align="center">
  <tr>
    <td align="center" width="45%">
      <img src="results/F1_curve.png" width="100%"><br>
      <em>SAM2</em>
    </td>
    <td align="center" width="45%">
      <img src="results/P_curve.png" width="100%"><br>
      <em>SAM2</em>
    </td>
  </tr>
</table>
</p>
<table align="center">
  <tr>
    <td align="center" width="45%">
      <img src="results/PR_curve.png" width="100%"><br>
      <em>SAM2</em>
    </td>
    <td align="center" width="45%">
      <img src="results/R_curve.png" width="100%"><br>
      <em>SAM2</em>
    </td>
  </tr>
</table>

# Change the source code a bit to make it more clear
</p>
<table align="center">
  <tr>
    <td align="center" width="45%">
      <img src="replace_source_code_object_counter.png" width="100%"><br>
      <em>object_counter.py</em>
    </td>
    <td align="center" width="45%">
      <img src="replace_source_code_solutions.png" width="100%"><br>
      <em>solutions.py</em>
    </td>
  </tr>
</table>
</p>

<p align="center">
  <img src="replace_source_code_solutions1.png" width="100%" alt="idea"/>
  <em>solutions.py</em>
</p>

# Result after changing a little source code

<p align="center">
  📺 <strong>Xem demo đếm xe bằng YOLO + SAM2</strong>
</p>
<p align="center">
  <a href="https://www.youtube.com/watch?v=ZYELfCVmh60">
    <img src="https://img.youtube.com/vi/ZYELfCVmh60/0.jpg" alt="Watch the video" width="60%" />
  </a>
</p>
