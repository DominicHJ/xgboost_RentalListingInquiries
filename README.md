## xgboost_RentalListingInquiries

### 1 简介  
使用xgboost在Kaggle 2017 Rental Listing Inquiries 数据集上进行参数调优，主要包括：  
- 初步确定弱学习器数目  
- 树的最大深度（max_depth）参数调优  
- min_children_weight调优  
- 正则参数调优  
- 弱学习器数目重新调整  
- 行列重采样参数调整  
- 调用模型进行测试  
- 生成测试结果文件  
  
### 2 数据集介绍  
#### Kaggle2017——Rental Listing Inquiries     
该数据集来自Kaggle 2017年举办的Rental Listing Inquiries分类竞赛数据，需要根据公寓的特征来预测其受欢迎程度（用户感兴趣程度分为高、中、低三类）。其中房屋的特征x共有14维，响应值y为用户对该公寓的感兴趣程度。评价标准为logloss。  
数据链接：https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries  
数据分析示例：https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries/kernels  
竞赛官网：https://www.kaggle.com/c/two-sigma-connect-rental-listing-inquiries/data   
