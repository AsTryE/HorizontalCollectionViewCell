# HorizontalCollectionViewCell
添加一个可以横向滚动的collectionView到自定义tableviewcell中，可以更改自定义背景，用于显示每行内容较多的表格数据，具体效果看截图
用法:  

  1.自定义cell，可以用代码，也可以通过故事版自定义（推荐），在右边的属性栏，关联 HorizontalTableViewCell类既可。  
  2.在 ### - (UITableViewCell *)tableView:(UITableView *)tableView cellForRowAtIndexPath:(NSIndexPath *)indexPath### 方法内    
    HorizontalTableViewCell * cell = [tableView dequeueReusableCellWithIdentifier:@"horizontalcellheadIdentifier"   forIndexPath:indexPath];  
        cell.labelBackgroundColor = [UIColor grayColor];  
        cell.textArray = @[@"姓名",@"学号",@"年龄",@"毕业学校",@"学历"];  
        [cell confiSelf];  
      数据，返回cell即可，可以设置不同cell的 'labelBackgroundColor' 属性 达到标题行的效果。  
  具体用法看例子。  
  第一张图片  
  
   ![image](https://github.com/804145113/HorizontalCollectionViewCell/blob/master/iOS%20Simulator%20Screen%20Shot%202015%E5%B9%B44%E6%9C%8828%E6%97%A5%20%E4%B8%8B%E5%8D%8810.31.33.png)   
     
     第二张图片  
     
   ![image](https://github.com/804145113/HorizontalCollectionViewCell/blob/master/iOS%20Simulator%20Screen%20Shot%202015%E5%B9%B44%E6%9C%8828%E6%97%A5%20%E4%B8%8B%E5%8D%8810.31.44.png)
