## 🛠️ Installation

See [INSTALL.md](INSTALL.md)

## 👨‍🏫 Get Started 
Running the following shell can start a gradio service:
```shell
git clone https://github.com/facebookresearch/segment-anything
pip install -r requirements.txt
python -u app.py --load "HuskyVQA_cuda:0,SegmentAnything_cuda:0,ImageOCRRecognition_cuda:0" --port 3456
```

if you want to enable the voice assistant, please use `openssl` to generate the certificate:
```shell
mkdir certificate
openssl req -x509 -newkey rsa:4096 -keyout certificate/key.pem -out certificate/cert.pem -sha256 -days 365 -nodes
```

and then run:
```shell
python -u app.py --load "HuskyVQA_cuda:0,SegmentAnything_cuda:0,ImageOCRRecognition_cuda:0" --port 3456 --https
```


## 🎫 License

This project is released under the [Apache 2.0 license](LICENSE). 

## 🖊️ Citation

If you find this project useful in your research, please consider cite:

```BibTeX
@article{2023interngpt,
  title={InternGPT: Solving Vision-Centric Tasks by Interacting with ChatGPT Beyond Language},
  author={Liu, Zhaoyang and He, Yinan and Wang, Wenhai and Wang, Weiyun and Wang, Yi and Chen, Shoufa and Zhang, Qinglong and Yang, Yang and Li, Qingyun and Yu, Jiashuo and others},
  journal={arXiv preprint arXiv:2305.05662},
  year={2023}
}
```

## 🤝 Acknowledgement
Thanks to the open source of the following projects:

[Hugging Face](https://github.com/huggingface) &#8194;
[LangChain](https://github.com/hwchase17/langchain) &#8194;
[TaskMatrix](https://github.com/microsoft/TaskMatrix) &#8194;
[SAM](https://github.com/facebookresearch/segment-anything) &#8194;
[Stable Diffusion](https://github.com/CompVis/stable-diffusion) &#8194; 
[ControlNet](https://github.com/lllyasviel/ControlNet) &#8194; 
[InstructPix2Pix](https://github.com/timothybrooks/instruct-pix2pix) &#8194; 
[BLIP](https://github.com/salesforce/BLIP) &#8194;
[Latent Diffusion Models](https://github.com/CompVis/latent-diffusion) &#8194;
[EasyOCR](https://github.com/JaidedAI/EasyOCR)&#8194;
[ImageBind](https://github.com/facebookresearch/ImageBind) &#8194;
[DragGAN](https://github.com/XingangPan/DragGAN) &#8194;

Welcome to discuss with us and continuously improve the user experience of InternGPT.

WeChat QR Code:

<p align="center"><img src="https://github.com/OpenGVLab/InternGPT/assets/8529570/60749865-1d9b-4e4e-8958-c7587c7adc5c" width="300"></p>



