### 机器人感知与控制期末大作业，借鉴https://github.com/yanx27/Pointnet_Pointnet2_pytorch
### 数据集链接：https://pan.baidu.com/s/1So4rCj35WuxgFa2y2ikwlg?pwd=1111 提取码：1111 
1、下载数据集并解压到 data/s3dis/Stanford3dDataset_v1.2_Aligned_Version  
2、数据预处理 在data_utils文件夹运行：  
python collect_indoor3d_data.py  
3、运行程序 以Area_5为测试集  
正式训练：python train_semseg.py --model pointnet2_sem_seg --test_area 5 --log_dir pointnet2_sem_seg  
测试：python test_semseg.py --log_dir pointnet2_sem_seg --test_area 5 --visual  
可以在log/sem_seg/pointnet2_sem_seg/visual/文件夹下看测试输出.obj文件（下个meshlab打开）
