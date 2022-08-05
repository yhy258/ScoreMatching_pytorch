# NCSN_pytorch
## 1. Standard NCSN.
**Result, MNIST Dataset**
3000 iteration  
![image](https://user-images.githubusercontent.com/33916246/169830113-2a0207aa-89ed-448f-b760-796f931a42c5.png)
  
   
6000 iteration  
![image](https://user-images.githubusercontent.com/33916246/169830195-4be8d3a2-066f-44ff-9e2e-669b108544af.png)  
   
   
9000 iteration  
![image](https://user-images.githubusercontent.com/33916246/169830298-10c18460-9189-4dcb-9667-a728acaa1867.png)  
   
   
12000 iteration  
![image](https://user-images.githubusercontent.com/33916246/169830346-1967dbd9-2226-48d5-8fc3-7fb519e78121.png)

## 2. VESDE
Code : https://github.com/yhy258/NCSN_pytorch/blob/main/VE_SDE_tutorial.ipynb  
Paper : https://openreview.net/pdf?id=PxTIG12RRHS  

## 3. Solving Inverse Problem In Medical Imaging With Score Based Generative Model
Code : https://github.com/yhy258/NCSN_pytorch/blob/main/Solving_Inverse_Problem_Given_Partial_Measurement.ipynb  
Paper : https://openreview.net/pdf?id=vaRCHVj0uGI  
본 코드에서 사용한 모델은 official code와 형태를 최대한 비슷하게 가져가려했으나, 코랩 프로로 돌리기 어려워 다소 간소화된 모델로 구성했습니다.  
그리고 official code에서는 fir filter를 사용하고 있으나 본 코드에서는 nearest 방법으로 sampling을 진행합니다.  
모델 내부에서 Downsampling -> Upsampling을 거쳐 의도와 맞는 노이즈를 생성해야하는 Unet의 특성 상 이러한 샘플링 방법은 좋지 않을 수 있다고 생각됩니다.  
실제로 본 코드를 통해 생성된 이미지들의 명도가 더 높음은 경향을 띔을 알 수 있고, 본 논문에서 제시하는만큼의 성능을 보이지는 못합니다.  
