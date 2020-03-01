# Learning-Robust-3D-Face-Reconstruction-and-Discriminative-Identity-Representation
This repo holds the pytorch improved version of the paper: [Learning-Robust-3D-Face-Reconstruction-and-Discriminative-Identity-Representation](https://arxiv.org/abs/1905.06505)  
# Getting started  
Requirements  
. Pytorch >=1.0  
. Python >= 3.6  
. Platform: Linux  
# Usage  
1. Clone this repo  
git clone https://github.com/Cluoyao/Learning-Robust-3D-Face-Reconstruction-and-Discriminative-Identity-Representation.git  
2. Training dataset  
Firstly, download train and test dataset train_aug_120x120.zip [Baidu Yun](https://pan.baidu.com/s/19QNGst2E1pRKL7Dtx_L1MA?errno=0&errmsg=Auth%20Login%20Sucess&&bduss=&ssnerror=0&traceid=) or [Google Drive](https://drive.google.com/file/d/17LfvBZFAeXt0ACPnVckfdrLTMHUpIQqE/view) and AFLW-2000-3D dataset [Bidu Yun](https://pan.baidu.com/s/1DTVGCG5k0jjjhOc8GcSLOw) or [Google Drive](https://drive.google.com/file/d/1r_ciJ1M0BSRTwndIBt42GlPFRv6CvvEP/view?usp=sharing)     
Then, download pre-trained model in [Baidu Yun](https://pan.baidu.com/s/1xLSke_X6CBt9SZwazLoOZg) Keywords:pymr, and put it into training_debug/logs  
After that, you can run the verify_recognition.py to test face recognition.
3. Training  
Firstly, download train.configs.zip flie [Baidu Yun](https://pan.baidu.com/s/10Zyy8C0ld4ipI9z_ZFSUQw) Keywords：tjec,and then put it in SCNN-master folder.Document organization relationship as follow：  
SCNN-master--｜-train.configs  
             ｜-train_debug  
             ｜-...  
After that, you can run the train_sia_network.py, get the first model, then you can run the wpdc＋shp_contrain.py and modify variable pre_model_params_path with former's path, then wpdc＋identify＋shp_contrain.py...
