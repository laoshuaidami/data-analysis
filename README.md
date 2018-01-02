# data-analysis
利用python进行数据分析
 假设由数据ex1.csv
import pandas as pd
df = pd.read_csv('ex1.csv')#读取数据
df = pd.read_csv('ex1.csv'，header=None)#读取数据,表头为空
df = pd.read_table('ex1.csv'，sep=',')#也可以读取数据，但是必须指定分隔符为，即sep=','
df.info()#查看数据详细信息
df.shape#查看数据结构
pd.read_csv('ex1.csv',index_col='message')#制定message列为索引列
df.describe()#描述信息内容
如果想要读取excel，需要pip install xlrd
df.to_csv('df1.csv')#将df保存为df1的csv文件
--列表方法
1.list1.extend(list2)#把列表1与列表2合并
这里总结一下，首先是append和extend的区别：append是把元素添加到一个list里，extend是把两个list结合在一起。
然后是extend和+的区别：+是创建了一个新的list并返回，运算量大，extend是在原本的list上做了更改，运算量小。
