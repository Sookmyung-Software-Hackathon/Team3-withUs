# 실행 방법
## #1 WEB CAM   
Open ``instant-noodle-webcam.ipynb`` with local jupyter notebook  
### Required   
- torch version 1.8.0 이상   
- CUDA 11.1 이상   
- **Web Cam 필수**  

### Parameter   
- ``weights_path`` : best.pt의 절대경로(폴더 위치: instant-noodle\yolov5\runs\train\noodle-result5\weights\best.pt)

## #2 TEST IMAGE
Open ``instant_noodel_test_img.ipynb`` with Colaboratory  
1. Google Drive ``/content/drive/Mydrive`` 경로에 ``instant-noodle`` 폴더 업로드   
2. 각 Cell 실행
3. detect.py 실행 확인 방법   
```python
from IPython.display import Image
import os
val_img_path = img_list[47]
weights_path = '/content/drive/MyDrive/instant-noodle/yolov5/runs/train/noodle-result5/weights/best.pt'
!python detect.py --weights "{weights_path}" --img 416 --conf 0.5 --source "{val_img_path}"
detect_img_path = '/content/drive/MyDrive/instant-noodle/yolov5/runs/detect/exp'
```   
위의 Cell 실행 후 'Results saved to runs/detect/**exp**'의 경로에 저장되었으므로, 해당 위치에서 확인 가능하다.   
4. cv2_imshow 사용시 ``Results saved to runs/detect/**exp**/(이미지 파일 이름)``으로 작성해야 확인할 수 있다.   

### Parameter   
- ``val_img_path`` : test images의 경로를 저장한 list
- ``detect_img_path`` : test images 실행 결과 이미지를 저장한 폴더의 경로   
   
## Model 학습 진행 상황
![image](https://user-images.githubusercontent.com/90624848/187072399-747700bd-8631-4a15-9aa9-3380028d12ac.png)

  
   
# 기획서
　　　　　　　　　　　　　　　　　　　　　　　[노션링크](https://eggplant-raccoon-ce3.notion.site/Team3-00e3f6dd0df14e03b7a9c2ed24b3b46f)
![001](https://user-images.githubusercontent.com/90624848/187071534-618aafc1-3055-40d0-b39e-e9bbf661a67e.jpg)
![002](https://user-images.githubusercontent.com/90624848/187071537-a89f5241-07ee-4369-ba0a-01fc15913eb7.jpg)
![003](https://user-images.githubusercontent.com/90624848/187071538-59c7d8db-ff9a-4610-91da-978d30c05b32.jpg)
![004](https://user-images.githubusercontent.com/90624848/187071539-a41033f6-b341-4585-af80-fb5d4004c52f.jpg)
![005](https://user-images.githubusercontent.com/90624848/187071541-de7e705b-f248-4d25-ae87-0a552d20c7ee.jpg)
![Noodle Freedom-006](https://user-images.githubusercontent.com/90624848/187249833-d5e3ac67-afc3-46a3-95ce-8a79b4f6deec.jpg)
![Noodle Freedom-007](https://user-images.githubusercontent.com/90624848/187249675-f4ba2b88-9446-4de9-9f03-86e42b73a7fd.jpg)

