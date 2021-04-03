# 开始训练
```pythonr
python run_pretrain.py \
--device_target {your device} \
--device_id {your device id} \
--enable_graph_kernel true \
--data_dir {your data dir}      
```

# 加载模型

``` python
python run_pretrain.py \
--device_target {your device} \
--device_id {your device id} \
--enable_graph_kernel true \
--data_dir {your data dir} \
--load_checkpoint_path {yout cpkt path}
```

#### enable_graph_kernel true
可以图加速算子，可以提升模型的运算效率，接近3成

#### data_dir
data_dir只需要给定文件夹就可以，他会遍历目录下所有的tfrecord文件

#### train_steps
原始全部数据完成一个epoch的训练可能需要2-3天
单卡telsaV100，因此建议使用--train_steps 10
比如只训练10步，用来测试模型能否正常运行即可






