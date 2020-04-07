## Dataset related to 3D face

**300W-3D-Face** [Link](http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/main.htm)

파일 구성

~~~
AFW : AFW dataset is built using Flickr images. It has 205 images with 473 labeled faces. For each face, annotations include a rectangular bounding box, 6 landmarks and the pose angles.
HELEN : Face landmark dataset
IBUG : Face detection dataset
LFPW : Face landmark dataset
~~~

각 폴더 내에는 mat 파일이 있고 Fitted_Face 데이터에 3D 정점 정보가 있음
The number of vertices of fitted face : 53215



**300W-3D** [Link](http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/main.htm)

The fitted 3D Morphable Model (3DMM) parameters of 300W samples

Image와 mat 파일이 1 set으로 존재

Mat file 구성

~~~
pt2d : 68 landmark points
roi, Illum_Para, Color_Para, Tex_Para, Shape_Para, Exp_Para, Pose_Para
~~~



**300W-LP** [Link](http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/main.htm)

The synthesized large-pose face images from 300W



**AFLW2000-3D** [Link](http://www.cbsr.ia.ac.cn/users/xiangyuzhu/projects/3DDFA/main.htm)

The fitted 3D faces of the first 2000 AFLW samples, which can be used for 3D face alignment evaluation



**CASIA-WebFace** [Link](https://drive.google.com/file/d/1Of_EVz-yHV7QVWQGihYfvtny9Ne8qXVz/view) : 10,575 subjects with over 494k images

CASIA WebFace Facial dataset of 453,453 images over 10,575 identities after face detection. Requires some filtering for quality.



**UV-GAN dataset** [Link](https://www.dropbox.com/sh/fs03rwy4i67pr1h/AAB2y6XGHITeWMhgs6lyB3o0a?dl=0)

파일 구성

~~~
image_jpg.tar : original image (37710)
3dmm_mask_png.tar : 3DMM fitting visible masks (37710) - 0,1로 된 mask vectors - png
3dmm_para.tar : 3DMM fitting parameters (37710)
3dmm_UV_jpg.tar : 3DMM fitting incompleted appearance maps (37710)
Completed_UV.tar : Completed UV appearance maps, pseudo ground truth (2514, 377*595*3)
3dmm_obj.tar : 3DMM fitting shape (2514)
landmark_pts.tar : annotated landmarks (37710)
Visualise_demo.tar
~~~

The number of vertices of 3dmm_obj  : 53215



**NoW dataset** [Link](https://ringnet.is.tue.mpg.de/en)

파일 구성

~~~
NoW Dataset
├── annotations.png : 3D face mesh에서 7개의 points
├── subjects_id.txt : subject 폴더 list
├── detected_face : 100 subjects의 folder
    ├── multiview_expression : neutral하지 않은 남이 찍어준 5장 이상의 사진
    ├── multiview_neutral : neutral한 남이 찍어준 5장 이상의 사진
    ├── multiview_occulations : 선글라스를 낀 채로 남이 찍어준 5장 이상의 사진
    └── selfie : 본인이 찍은 1장 이상의 사진
└── iphone_pictures : 100 subjects의 folder
    ├── multiview_expression : Bounding box 좌표 (top, left, right, bottom) - npy
    ├── multiview_neutral : Bounding box 좌표 (top, left, right, bottom) - npy
    ├── multiview_occulations : Bounding box 좌표 (top, left, right, bottom) - npy
    └── selfie : Bounding box 좌표 (top, left, right, bottom) - npy

Pre-trained Model (model.zip) : pretrained ringnet network weights
Validation Set (imagepaths validation.txt) : validation image list
Test Set (imagepaths test.txt) : test image list
Validation Set Scans : 29588개의 정점을 가진 각 subject의 non-preprocessed face scan
Validation Set Scans Landmarks : annotations.png와 같이 찍은 points - pp (Picked points)
~~~

The number of vertices of validation set scan : 29588



**Basel Face Model 2019 (BFM)** [Link](https://faces.dmi.unibas.ch/bfm/bfm2019.html)

파일 구성

~~~
model2019_fullHead.h5 : Full head model, the statistics for the back of the head based on little data and heuristics
model2019_bfm.h5 : Model masked similar to the original Basel Face Model mask
model2019_face12.h5 : Model cropped to the face region
model2019_fullHead_lvl2.ply : Mid resolution mesh
model2019_fullHead_lvl1.ply : Lowest resolution mesh
model2019_mouthOnly.ply : Mesh covering only the inner part of the mouth
model2019_textureMapping : Texture mapping file for our parametric data generator
~~~

The number of vertices of mid resolution mesh : 14581
The number of vertices of lowest resolution mesh : 3658
The number of vertices of mouth only mesh : 1609

