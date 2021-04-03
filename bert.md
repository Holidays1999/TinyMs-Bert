# for run_pretrain.py

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



