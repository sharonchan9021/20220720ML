# [Towards Building an Intelligent Anti-Malware System](https://arxiv.org/abs/1801.00318)
- A Deep Learning Approach using Support Vector Machine (SVM) for Malware Classification
- [GITHUB]()

## Data Set資料集
- Malimg dataset (Nataraj et al., 2011) 


#
```
git clone https://github.com/AFAgarap/malware-classification.git/

cd malware-classification

!sudo chmod +x setup.sh

修改requirements.txt
tensorflow_gpu==1.15.4
numpy==1.16.0
scikit_learn==0.19.1
tensorflow==1.15.4

!wget https://raw.githubusercontent.com/8wingflying/20220720/main/week4_machineLearning/MLSecurity/requirements.txt

!./bash setup.sh
```

```
!python3 main.py --model 1 --dataset ./dataset/malimg.npz --num_epochs 100 --penalty_parameter 10 --checkpoint_path ./checkpoint/ --log_path ./logs/ --result_path ./results/
```
