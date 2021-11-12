

### Introduction 
&ensp; &ensp; &ensp; &ensp; As far as we have surveyed, crack datasets available on internet are mostly 
focused on roads and building walls, which usually do not involved with very 
complex textures. Besides that, images in those datasets are mostly captured by 
consumer's devices like cellphones, with little restrictions on capture distance or 
angles, and all that makes pixel resolutions vary. Meanwhile, our country's guiding 
principles on building structures' visual inspection holds a standard that cracks with 
width above 0.1mm should all be noticed.

&ensp; &ensp; &ensp; &ensp; So, we published our crack dataset DroneCapturedTinyCrackDataset( DCTCD ) to solve problems all above. Our dataset is 
obtained with our company's drones which is designed for accurate crack detection in unreachable places like bridge beams or pier inner walls,lightning devices are equipped for 
all day usage. Besides, photo distances and angle are controlled to ensure 0.1mm resolution per pixel 
highest. Complex textures like scrawls, efflorenscenes are 
involved, as well as image degradation factors like motion blur, defocus blur, ISO 
noises, color jitter etc, which all makes our dataset much closer to actual 
engineering application;
### Data qualification 
&ensp; &ensp; &ensp; &ensp;We found that the more complex image background texture is, the more 
difficult it is for crack classification. In order to quantify crack classification’s 
difficulty, canny edge filters are used to generate a corresponding edge image, the 
total sum of edge image' s gray value are calculated and then divided with pixels' 
sum of the edge image, to produce a factor as we called edge complexity. The larger 
the factor is, the more difficult it is for crack classification
### Demos 
&ensp;  &ensp;According to this edge complexity factor, we divided our crack dataset into five folds, 
from H1 to H5. H1 is the simplest, H5 is the hardest. Each folder contains 50 crack 
images which dimenesion are all 512x512x3; we show some of our samples below.
     ![img_5.png](https://github.com/JY-AI-Tech/CrackDataset/blob/main/img_5.png)
### Crack Dataset Attribute
&ensp; &ensp; &ensp; &ensp; Detail descriptions about our crack datasets are in the table
<br>
     
|  Attribute     | Description   |
| :---        |    :----:   |
| Dataset Name      |     DroneCapturedTinyCrackDataset (DCTCD)  |
| Capture Drone   | JiaYing JYT-790       |
| Photo Angle   |  30°-90°     |
| Illumination intensity   |  1000+Lux     |
| Location   |    Bridge beam、Pier inner wall |
| Degradation Factor   |   Motion Blur、Defocus、 color jitter 、ISO noise    |
| Background  |    Scrawl、Efflorenscenes、 Surface Corrosion  |
| Image resolution  | 0.1mm-0.2mm per pixel    |


### Download:
You can also download the pretrained model from the following link,
[BaiduYunPan(Code:JYAI)](https://pan.baidu.com/s/1lggZx5sAJVjHv-_y3Qz0CA) 
### Contaction:
 Doc MingPeng.Li  &ensp; &ensp;   Email Address mpli@whu.edu.cn 
