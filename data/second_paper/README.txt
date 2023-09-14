按照如下方式设计文件结构：

- 数据类型
----- raw
    ----- soybean
    ----- maize
----- precessed
    ----- soybean
    ----- maize

最终整理可以直接输入进模型的数据是：
处理了物候的一张整表
D:\论文-产量趋势利用\数据\alldata_soybean.csv
D:\论文-产量趋势利用\数据\alldata_maize.csv

删除['Value','County','irrigated soybean area','soybean area']和包含'LE','30d','shortwave','90d','RVI','Lai','Fpar','WDRVI'的列，
去除大部分缺失行
D:\论文-产量趋势利用\数据\input_maize.csv
D:\论文-产量趋势利用\数据\input_soybean.csv

添加经纬度
连接1980年以来的产量
计算了EXP2、EXP3、EXP20、EXP30试验列
D:\论文-产量趋势利用\数据\input_maize_exp.csv
D:\论文-产量趋势利用\数据\input_soybean_exp.csv

对把平均产量作为特征的年份进行实验
D:\论文-产量趋势利用\数据\input_maize_exp_ave.csv
D:\论文-产量趋势利用\数据\input_soybean_exp_ave.csv

对把线性趋势产量作为特征的年份进行实验
D:\论文-产量趋势利用\数据\input_maize_exp_lin.csv
D:\论文-产量趋势利用\数据\input_soybean_exp_lin.csv