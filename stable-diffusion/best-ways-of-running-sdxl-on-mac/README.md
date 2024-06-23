# Best Ways of Running SD on Mac

Stable Diffusion (SD) has become a popular tool for AI-generated art. As an open-source solution, it can be run locally on your Mac without internet connectivity. This tutorial will cover the best ways to run SDXL models on your Mac.

If you prefer learning through a visual approach or want to gain additional insight into this topic, be sure to check out my YouTube video on this subject!

[![best ways of running SDXL on Mac](/stable-diffusion/best-ways-of-running-sdxl-on-mac/images/running-sdxl-on-mac.png)](https://youtu.be/TRf4Pa4IfJ0)


## Options

### Stable Diffusion Web UI by Automatic-1111

* Pros:
	+ Highly versatile, allowing text-to-image generation, image-to-image generation, and more
	+ Extensive customization options
	+ Supports image optimizers like ControlNet, refiners, or VAE
	+ Open-source, ensuring continuous review and improvement from the developer community
* Cons:
	+ Sluggish performance with SDXL models
	+ [Installation process](/stable-diffusion/install-automatic-1111/README.md) requires complex steps

### ComfyUI

* Pros:
	+ Faster performance compared to Automatic-1111
	+ Great flexibility in customization options
	+ Offers transparent visibility into its operations
	+ Open-source and free to use
* Cons:
	+ Requires a learning curve to become comfortable with the tool
	+ [Installation process](/stable-diffusion/install-comfyui/README.md) is not intuitive
	+ May have limitations on devices with limited GPU power

### Draw Things App

* Pros:
	+ Optimized for CoreML, enabling efficient execution of machine learning models on Apple devices
	+ Free to download and use (from the app store)
	+ Supports Stable Diffusion models 1, 2, and SDXL
	+ User-friendly interface requiring no complicated installation steps
* Cons:
	+ May have limitations in fine-tuning your own models or utilizing third-party applications

[Link to the Draw Things Website](https://drawthings.ai/)

## Conclusion

The choice of tool depends on your specific requirements. If you prioritize straightforward image generation without a learning curve, Draw Things is the ideal option. For those seeking additional features like fine-tuning their own model or using text-to-video functionalities and available extensions, ComfyUI may be the better choice.

Remember that there are other tools available for running Stable Diffusion locally, but they either come with a price tag or lack support for SDXL models.