1
要求：
安装python3。
安装tensorflow（在1.3.0、1.4.0、1.5.0、1.6.0、1.7.0版上测试）。
安装tensorflow工具包Neurogym（运行pip install git+https://github.com/JiahuiYu/neuralgym）。
2.
训练：
准备训练图像文件列表并对其进行随机播放（示例）。
修改inpaint.yml以设置DATA_FLIST，LOG_DIR，IMG_SHAPES和其他参数。
运行python train.py。
3.
继续训练：
修改MODEL_RESTORE标志inpaint.yml。例如，MODEL_RESTORE：20180115220926508503_places2_model。
运行python train.py。
4.
测试：
运行python test.py --image examples/input.png --mask examples/mask.png --output examples/output.png --checkpoint model_logs/your_model_dir。
#demo
# ImageInpainting
