# Audio Steganalysis with CNN
@ Author: **Wang Yuntao (Charles_wyt)** <br>
@ Email: wangyuntao2@iie.ac.cn <br>
Hope we can have a happy communication.

This project is a tensorflow implementation of recent work, you can also design your own network via this platform.
+ [CNN-based Steganalysis of MP3 Steganography in the Entropy
Code Domain](https://github.com/Charleswyt/tf_audio_steganalysis/tree/master/paper/CNN-based%20Steganalysis%20of%20MP3%20Steganography%20in%20the%20Entropy%20Code%20Domain) [[IH & MMSec](https://www.ihmmsec.org/) 2018, Best Paper Award]
**[[paper (ACM)](https://dl.acm.org/citation.cfm?id=3206011)]**
**[[paper (pdf)](http://www.media-security.net/?p=809)]**
**[[dataset](https://github.com/Charleswyt/tf_audio_steganalysis/tree/master/paper)]**

## Necessary Package
tensorflow-gpu==1.4 or later, numpy, pandas, matplotlib, scikit-image, scikit-learn, filetype, [**virtualenv**](https://charleswyt.github.io/2018/09/06/python%E8%99%9A%E6%8B%9F%E7%8E%AF%E5%A2%83%E5%AE%89%E8%A3%85%E5%8F%8A%E4%BD%BF%E7%94%A8/), [librosa](http://librosa.github.io/librosa/core.html) (depend on **[FFmpeg](http://www.ffmpeg.org/download.html)**)

You can use command **pip install -r requirements.txt** to install all packages mentioned above. If you don't want to change your version of tensorflow, you can use **virtualenv** to create a new python run environment.

## How to use
1. install [**python3.x**](https://www.python.org/) or [**Anaconda**](https://repo.continuum.io/archive/) and add the path into the environment variable
2. **GPU** run environment [**configure**](https://blog.csdn.net/yhaolpz/article/details/71375762?locationNum=14&fps=1) if train the network (optional)
3. install all dependent packages mentioned above (open **[setup](https://github.com/Charleswyt/tf_audio_steganalysis/tree/master/setup)/requirements.txt** and input "**pip install -r requirements**" into your cmd window)
4. **run** the code as the [**example**](https://github.com/Charleswyt/tf_audio_steganalysis/tree/master/config_file) as shows
5. use [**tensorboard**](http://wiki.jikexueyuan.com/project/tensorflow-zh/how_tos/graph_viz.html) to visualize the train process such as the **accuracy** and **loss curve** of train and validation. The command is "**tensorboard --logdir=/path/to/log-directory**"

## File description
ID      |   File                    |   Function
:-      |   :-                      |    :-
1       |   src                     |   source code
2       |   paper                   |   the PPT and brief introduction of our recent work
3       |   setup                   |   a **requirements.txt** in this folder, which is used to install all packages in this system
4       |   jupyter                 |   a folder for jupyter debug
5       |   data_processing         |   tools which are used for QMDCT coefficients extraction and dataset build
