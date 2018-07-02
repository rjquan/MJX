苗嘉旭 交接文档

1.	vggm_bn模型
a)	vggm_bn模型存放位置:
10.113.208.60:/home/miaojiaxu/train/vggm_re/vggm.prototxt
目前最好的模型：
vggm_bn_cam3_HWPtrain10_HYactor+Kako_Pre_iter_260000.caffemodel
b)	vggm_bn模型试验思路见 实验总结.pdf

2.	模型训练和测试
a)	模型训练和测试文档： 模型训练与测试.pdf   README_Evaluation.pdf


3.	Hash实验
a)	Hash实验结果文档：hash-h.xlsx，其中，hashloss实验 部分为使用hashloss.py训练的结果， hash阈值实验 部分为取阈值的结果。
b)	Hash 实验代码位置：
10.113.208.60:/home/miaojiaxu/train/hash_*(使用hashloss训练hash feature，结果在文档中，结果不如直接取阈值)
c)	Hash 实验思路： Learning to Hash.pptx

4.	衡阳数据库维护
a)	在10.175.100.250：/home/miaojiaxu/reid/db 中，存放衡阳的原始数据。是Cam3这个训练集的数据来源。
b)	衡阳数据统计表：ReID数据验收统计总表.xlsx

5.	数据存放
a)	目前所有训练集和测试集汇总：训练集&测试集汇总(2).xlsx

6.	评测统计
a)	目前跑过的千万库模型评测统计：评测统计(1).xlsx

7.	衡阳数据集实验
a)	关于衡阳30w数据集的构成，请参考cam3_data.xlsx
b)	该数据集所做的一系列实验结果：data实验0125.xlsx，实验0223.xlsx
c)	代码以及模型存放位置请见 data实验0125.xlsx ，实验0223.xlsx

8.	卡口数据实验
a)	卡口数据加入的实验结果：卡口数据加入训练集实验设置.xlsx
b)	代码以及模型存放位置请见卡口数据加入训练集实验设置.xlsx

9.	Mask实验
a)	Mask实验思路以及结果：MASK.xlsx
b)	代码存放位置：
10.113.208.60：/home/miaojiaxu/train/triplet/vggm_rgb
c)	测试代码：
10.113.208.60：/home/miaojiaxu/train/triplet/eval/getfeat.sh
d)	所需层：训练：data_layer_mask3.py      sampledata_mask.py
测试：
data_layer_mask3eval.py          sampledata_maskeval.py
10.	 测试集Mask提取
a)	代码位置: 10.113.208.60: /home/miaojiaxu/data/SegReID
 运行test_models_pva.sh
 
修改 OBJECT_IMAGE, OBJECT_TEST, SAVE_PATH
b)	10.113.208.60: /home/miaojiaxu/data/*_mask 这个文件夹中有所有测试集的mask文件。

11.	 训练集说明
a)	我所做实验的训练集保存在：10.113.208.60：/home/miaojiaxu/new_data 和 /home/miaojiaxu/new_data2
训练集的数据组成从名字中可以知道，如train_cam3_plus_person_HWP3 中包含 cam3数据和衡阳person数据 还有HWP三帧的数据。
目前最好的模型
vggm_bn_cam3_HWPtrain10_HYactor+Kako_Pre_iter_260000.caffemodel
所用的训练集位置：10.113.208.54：/home/miaojiaxu/new_data/train_cam3_HWPtrain10_HYactor+Kako



