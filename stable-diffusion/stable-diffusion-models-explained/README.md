# Stable Diffusion Models Explained

You've set up the Stable Diffusion Web UI locally, and now you're deciding on which model to use. For beginners, I suggest starting with a version 1 model. Yes, even though there are better models available right now! 

But what does choosing a model entail? What are the different model versions, and which one suits specific use cases? I'll explain all that in this tutorial.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![install stable diffuion](/stable-diffusion/stable-diffusion-models-explained/images/sd-models-explained-thumbnail.png)](https://youtu.be/U4JOCKlCPyg)


When picking a model, consider factors like version, size, style, and any additional installation steps.

## Model Version

The first factor is the model version. The three main versions of Stable Diffusion are version 1, version 2, and Stable Diffusion XL, also known as SDXL. 

Version 1 models are the first generation of Stable Diffusion models and they are [1.4](https://huggingface.co/CompVis/stable-diffusion-v-1-4-original) and the most renown one: version [1.5](https://huggingface.co/runwayml/stable-diffusion-v1-5) from RunwayML, which stands out as the best and most popular choice among the first-generation models.

Version 2 models consist of [2.0](https://huggingface.co/stabilityai/stable-diffusion-2) and [2.1](https://huggingface.co/stabilityai/stable-diffusion-2-1), with 2.1 notably representing a significant improvement over 2.0, particularly in its handling of negative prompts.

[SDXL](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0) are the newest generation of stable diffusion models. They are larger and more powerful, but also slower and more resource-intensive. 

## Model Size

The model's size impacts both the speed and image quality. Also, since you must download the models locally, it will take up space on your Mac. Larger models generally yield higher-quality images but are slower and demand more memory and storage. Smaller models are quicker and resource-efficient but might have lower resolution or more noise in the generated images. 

You can find a model's size indicated on the website where you download it. For example, if you visit Hugging Face to download the [Stable Diffusion v1.5 model](https://huggingface.co/runwayml/stable-diffusion-v1-5), you'll notice two available files: one at 4.27 GB and another at 7.7 GB.

![Image Size](/stable-diffusion/stable-diffusion-models-explained/images/model-size.png)

## Model Style

I'd like to clarify something before we dive into model styles. Up until now, I've mentioned stable diffusion base models, specifically generation 1, generation 2, and SDXL. Generation 1 models were created through collaboration between researchers from the CompVis Group at Ludwig Maximilian University of Munich and Runway. They were trained with computational resources provided by Stability AI and data from non-profit organizations. Stability AI later developed generation 2 models and SDXL.

Now, based on these three generations, anyone can fine-tune the base model by training it on specific images or styles. These fine-tuned models essentially stem from the base models, and this is where different styles come into play.

These models exhibit various styles and characteristics that influence how the generated images appear. Some models lean towards realism, while others embrace artistry or abstraction. Certain models are versatile, while others are specialized for particular domains or themes. You can judge a model's style by reviewing examples or reading its description.

![Base and Fine-Tuned Models](/stable-diffusion/stable-diffusion-models-explained/images/base-and-finetuned-models.png)

In fact, most models are still based on Stable Diffusion 1.5. For example, [Realistic Vision V5.1](https://civitai.com/models/4201?modelVersionId=6987) which produces very realistic portraits of people or [Anything V3](https://civitai.com/models/66?modelVersionId=75) which specializes in Anime images.

A model's specialization in a specific type of images doesn't mean you can't use it for other types of images. It simply means it produces the best results for the type of images it was fine-tuned on.

### Some Popular Stable Diffusion Models

These are some of the models that I have been using.

| Fine-Tuned Model                                  | Base Model            | Best for                                      | Example |
| -------------------------- | --------- | ------- | ------- |
| ----- |[stable-diffusion-v1-5](https://huggingface.co/runwayml/stable-diffusion-v1-5)| The best base model for beginners |![img](/stable-diffusion/stable-diffusion-models-explained/images/sd-v1_5-01.png)|
| ----- |[Stable Diffusion 2.1](https://huggingface.co/stabilityai/stable-diffusion-2-1)| The best base model in gen 2 |![img](/stable-diffusion/stable-diffusion-models-explained/images/sd-v2_1.png)|
| ----- |[Stable Diffusion XL](https://huggingface.co/stabilityai/stable-diffusion-xl-base-1.0)| SDXL, the latest base model from Stable Diffusion |![img](/stable-diffusion/stable-diffusion-models-explained/images/sdxl-image.png)|
|[Anything v3](https://huggingface.co/Linaqruf/anything-v3.0)|  Stable Diffusion V5.1 | The go-to model for anime art|![img](/stable-diffusion/stable-diffusion-models-explained/images/anything-v3.png)|
|[Realistic Vision V5.1](https://civitai.com/models/4201/realistic-vision-v51)| Stable Diffusion V5.1 | Produces realistic but not photorealistic images. Great for portraits! |![img](/stable-diffusion/stable-diffusion-models-explained/images/realistic-vision.png)|
|[Dreamshaper](https://civitai.com/models/4384?modelVersionId=128713)| Stable Diffusion V5.1 | Excellent photorealism model, but also good for Anime |![img](/stable-diffusion/stable-diffusion-models-explained/images/dreamshaper.png)|

## Additional Installation Steps

Depending on your choice of model, there might be some extra steps involved in using it.

### Installing Generation 1 Models

Generation 1 models are the simplest to employ with Stable Diffusion Web UI from AUTOMATIC1111. You download these models and place them in a dedicated model folder, refresh the UI, and you're ready to start generating images. When I mention "file," I'm referring to a checkpoint or safe tensors file.
- [Stable DIffusion 1.4](https://huggingface.co/CompVis/stable-diffusion-v-1-4-original) ([sd-v1-4.ckpt](https://huggingface.co/CompVis/stable-diffusion-v-1-4-original/resolve/main/sd-v1-4.ckpt))
- [Stable Diffusion 1.5](https://huggingface.co/runwayml/stable-diffusion-v1-5) ([v1-5-pruned-emaonly.ckpt](https://huggingface.co/runwayml/stable-diffusion-v1-5/resolve/main/v1-5-pruned-emaonly.ckpt))

### Installing Generation 2 Models 
Generation 2 models require more steps. For example, the base model Stable Diffusion 2.1 requires downloading a configuration file, renaming it to match the checkpoint file's name, and putting both files in the model folder for Stable Diffusion Web UI.
- [Stable Diffusion 2.0](https://huggingface.co/stabilityai/stable-diffusion-2) ([768-v-ema.ckpt](https://huggingface.co/stabilityai/stable-diffusion-2/resolve/main/768-v-ema.ckpt))
- [Stable Diffusion 2.1](https://huggingface.co/stabilityai/stable-diffusion-2-1) ([v2-1_768-ema-pruned.ckpt](https://huggingface.co/stabilityai/stable-diffusion-2-1/resolve/main/v2-1_768-ema-pruned.ckpt))

You can download the configuration file from [here](https://github.com/Stability-AI/stablediffusion/raw/main/configs/stable-diffusion/v2-inference-v.yaml). After downloading it, you must change the filename of the configuration file (which is a `.yml` file) to the filename of the model. So for model file `v2-1_768-ema-pruned.ckpt`, you must rename the configuration file to `v2-1_768-ema-pruned.yml` and put both files in the [model folder](/stable-diffusion/install-automatic-1111/README.md#download-the-model) for Stable Diffusion Web UI. 

### Installing SDXL

As for SDXL, it becomes even more complex. So far, I have not been able to run SDXL locally on my Mac without issues, especially since I only have 8GB of RAM. I have been running it on Google Colab instead.

## Popular Websites for Models

There are two excellent websites for downloading Stable Diffusion models.

I'd say that, in general, [Hugging Face](https://huggingface.co/models) is the top choice for getting the base models, while [Civit AI](https://civitai.com/models) is the go-to platform for derived or fine-tuned models.

## Conclusion

You might assume that opting for newer Stable Diffusion versions is the way to go. However, taking into account all the factors we've talked about, my suggestion for beginners is to **start with Stable Diffusion base model version 1.5 or its derivatives**. These models are the simplest to get started with, offering a quick and hassle-free setup, relatively small size, and they produce excellent images.

As you gain more experience, you can then consider transitioning to version 2 or SDXL.
