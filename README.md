# UIExPickerView
1.现在只支持1列数据,后续修改可以支持自定义列的数据。

只需要传入数组和frame即可得到选择的数据，不需要修改任何代码。 
UIExPickerView *pView = [[UIExPickerView alloc ] initWithFrame:CGRectMake(0, self.view.frame.size.height-200, self.view.frame.size.width, 200) arr:arr ];   
pView.delegate = self;  
[self.view addSubview:pView];  
//回调方法 
- (void)selectIndex:(NSInteger)index 
{ 
//根据索引取出传入数组的值    
NSLog(@"%ld",(long)index);
}
