domain adaptationʵ��
=============================

��Ŀ��cnn������ʵ����domain adaptation
��Ŀ�������������ģ�unsupervised domain adaptation by backpropagation  :
���ص�ַ��http://machinelearning.wustl.edu/mlpapers/paper_files/icml2015_ganin15.pdf

=============================
ʵ���ǻ���cnn����
CNN���������ģ�http://blog.csdn.net/u012162613/article/details/43225445
CNN������Դ��https://github.com/wepe/MachineLearning/blob/master/DeepLearning%20Tutorials/cnn_LeNet/convolutional_mlp_commentate.py

=============================
��Ŀ�ļ���ֻ���ĸ��ļ��У�SRC��data��result��reference

=============================
SRC�洢����Ŀ���е�Դ���룺
����˳��generate_data.py -> generateMNIST_SandMNIST_T.py -> cnn_~~~.py

generate_data.py:����mnist.pkl.gz����Ŀ�������ݼ���target~.pkl��st~.pkl������data/�£�
������generate_data.py���޸�theta��Դ���Ŀ����ͼƬ����ʱ�˵ı�������ֹ������Ĳ�����

generateMNIST_SandMNIST_T.py������source.pkl��target~.pkl��st~.pkl���ɲ���ͼƬ��������չʾ
ֻ������һ���֣�train,valid,test������10��ͼƬ��

cnn_ts_ts.py:��Դ����ѵ������Դ���ϲ���

cnn_ts_tt.py:��Դ����ѵ������Ŀ�����ϲ��ԣ���֤��ΪĿ�������ݣ�

cnn_tt_tt.py:��Ŀ������ѵ������Ŀ�����ϲ���

cnn_tst_ts.py:��Դ���Ŀ������ѵ������Ŀ�����ϲ��ԣ�Ҳ����ʹ����������Ӧ���ƣ�����֤����ΪĿ�������ݣ�
���������е���lmbda�������й�ʽ4��lambda��

����4���ļ�����������txt�ļ��У�����result/��

=============================
data�´�����Ŀ��Ҫ������ݣ�
�����г���ǰҪ���������ļ���BSR�ļ��У�imageMNIST_T�ļ��У�imageMNIST_S�ļ��У�mnist.pkl.gz, source.pkl

����BSR�ļ��У�
������Դ��http://www.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/BSR/BSR_bsds500.tgz
���ݼ����ܣ�https://www2.eecs.berkeley.edu/Research/Projects/CS/vision/grouping/resources.html#bsds500
�������֮��BSR_bsds500.tgz��ѹ������һ��BSR�ļ��У������BSR�ļ��зŵ�data�¾���

imageMNIST_S��imageMNIST_T:�����ļ��д洢generateMNIST_SandMNIST_T.py���ɵ�ͼƬ��
imageMNIST_S�洢Դ���ͼƬ
imageMNIST_T�洢Ŀ����ͼƬ
����ǰΪ�ռ���
imageMNIST_S��imageMNIST_T��������ͬ��ͼƬ���Ӧ

mnist.pkl.gz����mnist���ݼ�������ǰҪ���غ�
������Դ��http://www.iro.umontreal.ca/~lisa/deep/data/mnist/mnist.pkl.gz

source.pkl����mnist.pkl.gz�Ľ�ѹ�ļ�������ǰҪ��ѹ��


���к������st~.pkl��target~.pkl����data�£�
����~���ֱ�ʾtheta��ȡֵ

=============================
result�´������н��
���н���ļ�������ʽ�ʹ����ļ�������ʽ��ͬ

=============================
reference�´�����Ŀ����
unsupervised domain adaptation by backpropagation

=============================
��Ŀ���ڵ���Ҫ������
theta��Դ���������ͼƬͬ���ص�Ҷ�ֵ����ʱ��������˵ı�����
������4.1Results--MNIST->MNIST-M�е�ͼƬ���ɹ�ʽ������I1��I2����ʱ��I2����һ��theta������Դ���Ŀ����Ĳ�ࡣ
theta��0��1֮�䣬ԽС���ԽС��Խ����Խ��

lmbda�������й�ʽ4��lambda�������ڷ��򴫲������У������������ʧ��������ȡ���Ĳ������޸ĳ̶ȡ�
lmbda��0��1֮�䣬lmbdaԽС�������������ʧ��������ȡ���Ĳ������޸ĳ̶�ԽС��


