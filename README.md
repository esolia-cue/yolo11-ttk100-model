# About

This is a model based on yolo11 training 100 rounds with partial ttk100 data sets provides classification and detection for 45 classes in the ttk100 data set.  
[ttk100 data set - link](https://cg.cs.tsinghua.edu.cn/traffic-sign/tutorial.html)

The model runs on Utralytics YOLO Version(YOLO11) 
[Utralytics YOLO11 - link](https://github.com/ultralytics/ultralytics)

# Structure

## models
`models` directory is the model path follows the yolo training output format. 
the available model is `models.weights.best.pt` which is the best model after 100 rounds training, you can use it to do the inference or continue training based on it.

the files under models show the training log and the model behavior during the training process.

## data
`data.ttk100.yaml` is a demo data configuration file for the ttk100 data set, provides the class names and the class number.

dataset hasbeen splited into train and test set and they are all prescreened, so they did not contain the hole origin ttk100 data set.

dataset is not included in this repository, you can download it from the below link.
[dataset](https://pan.baidu.com/share/init?surl=1da9eDX188RMqawb_JncNg&pwd=1234)

# Thanks

Thanks for CSDN user [安全？？](https://blog.csdn.net/qq_40880583) for providing the preprocessed data set and the split script, you can find the blog here:
[TT100K数据集转yolo格式教程并分享做好的yolo格式数据集](https://blog.csdn.net/qq_40880583/article/details/136381785)
the download link upper is from the blog.

thanks my 4070-laptop for the training process.