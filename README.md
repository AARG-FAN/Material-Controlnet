# Material-Controlnet
A self trained Controlnet model for controlling materials

![微信截图_20240628184335](https://github.com/AARG-FAN/Material-Controlnet/assets/125116261/eca51ae0-2fe7-4b27-b9a6-1821939cad70)

# 1. Description:
This is the first controlnet model we trained
We are inspired by the CN model of semantic segmentation and hope to train a designer specific controllet model. Through this model, we can solve this pain point once and for all, so that we can obtain the results we want more accurately when using AI for drawing. Finally. After spending a long time manually annotating a lot of data and trained this controlnet, this problem has finally been solved! Today we have also opened up our CN material control model Material_control V0.7, and we will open up a better version depending on the situation in the future.

At present, the open version supports precise control of # 76380b (wood), # cd5c5c (brick), # 4c4c4c (concrete), # 00bfff (glass), and # c0c0c0 (metal). After multiple tests, it was found that the model can not only control the position and texture of materials, but also achieve excellent results with very simple prompts without Lora, which is something we did not expect.


![微信截图_20240630023717](https://github.com/AARG-FAN/Material-Controlnet/assets/125116261/1984d79b-9619-4ad3-9e0d-04ee70e5fb26)


Recommended large models: realistic models for architecture, all other types of large models are available

Recommended Controlnet weight: 1
Recommended tip word: You can write the desired materials or not, starting with "a modern building" and writing freely afterwards


# 2. How to use:

1. download the model here:https://huggingface.co/archifancy/Material_Control_Controlnet/tree/main
2. put the model into "stablediffuion-models-ControlNet" folder
3. paint the control image with the color I identified(# 76380b (wood), # cd5c5c (brick), # 4c4c4c (concrete), # 00bfff (glass), and # c0c0c0 (metal))
4. set the prepared control image as the input of controlent(both webui and comfyui work fine)
5. choose preprocesor as "none" and choose the controlnet model as the downloaded model
6. set the controlnet weight as around 1
7. set CKPT as LWarchi or dreamshaper as whatever you like
8. Generate

如何使用
1. 下载模型： https://huggingface.co/archifancy/Material_Control_Controlnet/tree/main
2. 将模型放入“stablediffusion-models-ControlNet”文件夹
3. 使用我标识的颜色绘制控制图像（#76380b（木材），#cd5c5c（砖块），#4c4c4c（混凝土），#00bfff（玻璃），和#c0c0c0（金属））
4. 将准备好的控制图像设置为ControlNet的输入（WebUI和ComfyUI都可以正常工作）
5. 选择预处理器为“none”，并选择下载的ControlNet模型
6. 将ControlNet权重设置为大约1
7. 将CKPT设置为LWarchi或dreamshaper，根据您的喜好选择
8. 生成

# 3. Examples:

![微信截图_20240628184405](https://github.com/AARG-FAN/Material-Controlnet/assets/125116261/10d60af8-cd4a-414f-bc55-0eb1b96c7325)

![微信截图_20240628184416](https://github.com/AARG-FAN/Material-Controlnet/assets/125116261/27fda64e-567f-4ecd-8230-c7d3f14dcf1b)

![微信截图_20240628184436](https://github.com/AARG-FAN/Material-Controlnet/assets/125116261/9231d98e-703c-45de-91c9-3dcaabdbac65)

![微信截图_20240628184428](https://github.com/AARG-FAN/Material-Controlnet/assets/125116261/bf4aa485-14f6-48b5-9e0b-794897b01e98)

# 4. License:
This model is for non-commercial use. If commercial use is required, please confirm with me: aargxufan@outlook.com
