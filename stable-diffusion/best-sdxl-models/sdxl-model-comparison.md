# SDXL Model Comparison

Most prompts were generated using [Leonardo AI](https://app.leonardo.ai/) Prompt Generator. However, I used Automatic1111 Stable Diffusion Web UI in Google Colab for image generation. I used the same prompts and seeds for all models.

I applied identical prompts and seeds across all images. However, I adhered to the recommended configurations and negative prompts specific to each model.

The images displayed are generated directly by the AI without any extra manipulation. There are no added negative prompts (except when suggested by the creators of the model), no inpainting, and no refining, except for the official SDXL version where I utilized the provided refiner file. All other models come with a built-in refiner. As a result, you may come across some images with extra limbs or other inconsistencies. Nevertheless, I felt it was fairest to preserve them in their original state for a more balanced comparison.

## Gorgon Alleyway
**Prompt:** In a dimly lit alleyway, a peculiar gorgon figure materializes, casting elongated shadows across the cracked pavement. This anomalous being, captured in a dreamlike street photography pastel tones photograph, presents a fusion of reality and fantasy. The image, while showcasing its intrinsic oddity, maintains a certain delicate elegance with soft hues and gentle brushstrokes. The meticulous attention to detail is evident in the intricate folds of the gorgon's flowing cloak, the ethereal wisps of smoke surrounding its head, and the enigmatic gleam in its mesmerizing eyes. Immersed in the picture, viewers will be engrossed by the extraordinary subject's enigmatic presence, provoking contemplation about the duality of existence and the allure of the mysterious.

**Seed:** 3719253140  

**Image Dimensions:** 1024 x 1024  

| Image               | ![00000-3719253140.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00000-3719253140.png) | ![00000-3719253140.png](/stable-diffusion/best-sdxl-models/images/copax/00000-3719253140.png) | ![00000-3719253140.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00000-3719253140.png) | ![00000-3719253140.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00000-3719253140.png) | ![00000-3719253140.png](/stable-diffusion/best-sdxl-models/images/realvis/00000-3719253140.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Nanotech Marvel
**Prompt:** This blood-curdling lustrous nanotechnology marvel in the anime is depicted in a hauntingly beautiful image, akin to a mesmerizing painting. Every intricate detail of this technological wonder is brought to life. Its surface glistens with a glossy sheen, reflecting an otherworldly iridescence that sends chills down your spine. The nanotechnology is expertly crafted, showcasing a predatory allure with sharp, gleaming edges that hint at its dangerous capabilities. The colors used in this image are vivid and intense, evoking a sense of both fascination and dread. This image captures the essence of a cutting-edge creation, leaving viewers in awe of its terrifying beauty.  

**Seed:** 2855127902  

**Image Dimensions:** 1024 x 1024  

| Image               | ![00001-2855127902.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00001-2855127902.png) | ![00001-2855127902.png](/stable-diffusion/best-sdxl-models/images/copax/00001-2855127902.png) | ![00001-2855127902.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00001-2855127902.png) | ![00001-2855127902.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00001-2855127902.png) | ![00001-2855127902.png](/stable-diffusion/best-sdxl-models/images/realvis/00001-2855127902.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Tech Elemental
**Prompt:** A mesmerizingly modernized embodiment of the elements, the tech-savvy elemental is portrayed in a pinhole cinematic photograph. This image, captured with precision and clarity, showcases a humanoid figure composed of swirling currents of electricity, glowing with vibrant shades of neon and piercing blues. The fine details accentuate the intricate circuitry that illuminates its robotic skeleton, while its luminous eyes exude an aura of cutting-edge innovation. The backdrop of the photograph, an industrialized cityscape bathed in the warm hues of a setting sun, adds depth and context to the scene. This remarkable artwork masterfully captures the seamless fusion of technology and elemental power.  

**Seed:** 2570845037  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00002-2570845037.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00002-2570845037.png) | ![00002-2570845037.png](/stable-diffusion/best-sdxl-models/images/copax/00002-2570845037.png) | ![00002-2570845037.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00002-2570845037.png) | ![00002-2570845037.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00002-2570845037.png) | ![00002-2570845037.png](/stable-diffusion/best-sdxl-models/images/realvis/00002-2570845037.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Glamorous Femme
**Prompt:** In an enchanting urban setting, towering skyscrapers loom in deep shadow as their neon lights pierce the night. A glamorous femme fatale, dressed in a form-fitting sequined gown, stands at the center of a dimly lit alley. The scene is captured in a stunningly detailed, digital painting. The artistry shines through in the intricate linework and meticulous shading, showcasing the talent of the artist. The image evokes an atmosphere of mystery and intrigue, drawing viewers into a captivating neo-noir narrative.  

**Seed:** 656694883  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00003-656694883.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00003-656694883.png) | ![00003-656694883.png](/stable-diffusion/best-sdxl-models/images/copax/00003-656694883.png) | ![00003-656694883.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00003-656694883.png) | ![00003-656694883.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00003-656694883.png) | ![00003-656694883.png](/stable-diffusion/best-sdxl-models/images/realvis/00003-656694883.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |

## Neural Network
**Prompt:** In a mesmerizingly surreal urban geometry photograph, a supernatural neural network emerges with an analog-inspired essence. The main subject of the image is a complex network of interconnected nodes resembling intertwining branches, illuminated by a soft, ethereal glow. Captured in high definition, the image vividly captures the intricate details of the neural network, showcasing its intricate, interwoven structure. The juxtaposition of the digital nature of the network with the organic feel of analog aesthetics adds a touch of enigmatic charm to the scene. 

**Seed:** 2617212831  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00004-2617212831.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00004-2617212831.png) | ![00004-2617212831.png](/stable-diffusion/best-sdxl-models/images/copax/00004-2617212831.png) | ![00004-2617212831.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00004-2617212831.png) | ![00004-2617212831.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00004-2617212831.png) | ![00004-2617212831.png](/stable-diffusion/best-sdxl-models/images/realvis/00004-2617212831.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Exquisite Portrait
**Prompt:** In a stunning close-up photograph, an exquisite woman takes center stage, her flawless features illuminated. Her mesmerizing eyes captivate with a sparkling emerald hue, complemented by long, luscious lashes. Her radiant smile reveals pearly white teeth framed by perfectly contoured lips. Silken, flowing locks cascade over her shoulders, their hues blending seamlessly from deep ebony to cascading chestnut. This high-quality image presents an awe-inspiring portrayal of a truly beautiful woman, showcasing her elegance and grace in vivid detail.  

**Seed:** 2492830952  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00005-2492830952.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00005-2492830952.png) | ![00005-2492830952.png](/stable-diffusion/best-sdxl-models/images/copax/00005-2492830952.png) | ![00005-2492830952.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00005-2492830952.png) | ![00005-2492830952.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00005-2492830952.png) | ![00005-2492830952.png](/stable-diffusion/best-sdxl-models/images/realvis/00005-2492830952.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Grotesque Cityscape
**Prompt:** In a strikingly grotesque cityscape painted in vibrant acrylic, the deranged fervor of its inhabitants is palpable. The main subject of the image is a towering cathedral-like structure, its windows dripping with an ominous golden glow, while gargoyles with twisted grins leer from every corner. The painting, meticulously detailed and expertly executed, gives the viewer an unsettling glimpse into the nightmarish intensity of this fanatical city.  

**Seed:** 887226551  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00006-887226551.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00006-887226551.png) | ![00006-887226551.png](/stable-diffusion/best-sdxl-models/images/copax/00006-887226551.png) | ![00006-887226551.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00006-887226551.png) | ![00006-887226551.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00006-887226551.png) | ![00006-887226551.png](/stable-diffusion/best-sdxl-models/images/realvis/00006-887226551.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Unsettling Ballerina
**Prompt:** In this ethereal virtual art gallery, an unsettling yet captivating presence takes center stage: a ghostly figure of a ballerina bowing gracefully on a stage of wispy fog. The image, a high fashion cinematic photograph, flawlessly captures the delicate movements of the dancer, her transparent form exuding an otherworldly elegance. Every detail is impeccably rendered, from the shimmering sequins adorning her flowing ballet dress to the ethereal glow emanating from her fingertips. The photograph's impeccable quality immerses viewers in a hauntingly beautiful world, where the boundaries between reality and fantasy blur in a mesmerizing dance.  

**Seed:** 2322571094  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00007-2322571094.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00007-2322571094.png) | ![00007-2322571094.png](/stable-diffusion/best-sdxl-models/images/copax/00007-2322571094.png) | ![00007-2322571094.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00007-2322571094.png) | ![00007-2322571094.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00007-2322571094.png) | ![00007-2322571094.png](/stable-diffusion/best-sdxl-models/images/realvis/00007-2322571094.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Vegan Ramen
**Prompt:** A visually striking image showcases a bowl of vegan ramen, capturing the essence of this beloved culinary delight. Skillfully captured in a high-resolution photograph, the bright and lively colors of the dish pop off the screen, inviting viewers to take a closer look. The steaming broth, teeming with aromatic spices, provides a tantalizing backdrop for the assortment of fresh and crisp vegetables. Each ingredient is meticulously arranged, from the velvety tofu cubes to the delicate slices of vibrant carrots, creating a feast for the eyes. This image exudes such remarkable clarity and attention to detail that one can practically taste the rich umami flavor and feel the comforting warmth emanating from the bowl.  

**Seed:** 1895783298  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00008-1895783298.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00008-1895783298.png) | ![00008-1895783298.png](/stable-diffusion/best-sdxl-models/images/copax/00008-1895783298.png) | ![00008-1895783298.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00008-1895783298.png) | ![00008-1895783298.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00008-1895783298.png) | ![00008-1895783298.png](/stable-diffusion/best-sdxl-models/images/realvis/00008-1895783298.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Beautiful Lady
**Prompt:** Beautiful lady, (freckles), big smile, ruby eyes, pigtails hair, dark makeup, hyperdetailed photography, soft light, head and shoulders portrait, cover  

**Seed:** 1272220565  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00009-1272220565.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00009-1272220565.png) | ![00009-1272220565.png](/stable-diffusion/best-sdxl-models/images/copax/00009-1272220565.png) | ![00009-1272220565.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00009-1272220565.png) | ![00009-1272220565.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00009-1272220565.png) | ![00009-1272220565.png](/stable-diffusion/best-sdxl-models/images/realvis/00009-1272220565.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |

## Lunar New Year Dragon
**Prompt:** A captivating image of a Chinese Lunar New Year dragon, possibly a photograph or a painting, that mesmerizes the viewers with its vibrant colors and intricate details. The majestic dragon is depicted in all its glory, adorned with beautifully adorned scales that shimmer in shades of gold and vermilion. Its mesmerizingly expressive eyes seem to spark with life, while its sinuous body coils elegantly to showcase its strength and power. The artist's skill is evident in every brushstroke or click of the camera, capturing the essence and magnificence of this legendary creature. This exceptional image undoubtedly transports the viewers into the enchanting world of Chinese mythology and cultural celebration.  

**Seed:** 1981171048  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00010-1981171048.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00010-1981171048.png) | ![00010-1981171048.png](/stable-diffusion/best-sdxl-models/images/copax/00010-1981171048.png) | ![00010-1981171048.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00010-1981171048.png) | ![00010-1981171048.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00010-1981171048.png) | ![00010-1981171048.png](/stable-diffusion/best-sdxl-models/images/realvis/00010-1981171048.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Chibli Art Style
**Prompt:** Photorealistic chibi art style, a beautiful woman in jeans and high heels, facing the viewers pretending to be scared, both hands on face, artistic, artist, simple volumtric light background, swirling clouds, ColorART, many cute ghosts with tongues out, chibi

**Seed:** 2222685910  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00012-2222685910.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00012-2222685910.png)           | ![00012-2222685910.png](/stable-diffusion/best-sdxl-models/images/copax/00012-2222685910.png)           | ![00012-2222685910.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00012-2222685910.png) | ![00012-2222685910.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00012-2222685910.png) | ![00012-2222685910.png](/stable-diffusion/best-sdxl-models/images/realvis/00012-2222685910.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Endearing Extraterrestrial
**Prompt:** A whimsically endearing extraterrestrial being, brimming with charm and appeal. This delightful creature, captured in a mesmerizing photograph, showcases its distinctive features: soft pastel fur, mesmerizingly large sparkly eyes, and an enchanting smile that instantly draws you in. The high resolution image, portrays the creature in exquisite detail, highlighting its vibrant colors and adorable form.  The bright colors accentuate its cuteness, evoking a sense of wonder and delight.  

**Seed:** 2674118466

**Image Dimensions:** 1024 x 1024  


| Image               | ![00013-2674118466.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00013-2674118466.png) | ![00013-2674118466.png](/stable-diffusion/best-sdxl-models/images/copax/00013-2674118466.png) | ![00013-2674118466.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00013-2674118466.png) | ![00013-2674118466.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00013-2674118466.png) | ![00013-2674118466.png](/stable-diffusion/best-sdxl-models/images/realvis/00013-2674118466.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Katana Girl
**Prompt:** (best quality, masterpiece), 1girl, katana, samurai, looking at viewer, dual wielding, tree, leaf

**Seed:** 552261060

**Image Dimensions:** 1024 x 1024   


| Image               | ![00014-552261060.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00014-552261060.png) | ![00014-552261060.png](/stable-diffusion/best-sdxl-models/images/copax/00014-552261060.png) | ![00014-552261060.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00014-552261060.png) | ![00014-552261060.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00014-552261060.png) | ![00014-552261060.png](/stable-diffusion/best-sdxl-models/images/realvis/00014-552261060.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Computer Bug
**Prompt:** A metallic insect constructed entirely out of a gleaming, state-of-the-art technology called ral-semiconductor, is seen through the lens of a magnifying glass resting on a sophisticated ral-semiconductor surface. The image, possibly a stunning photograph, encapsulates the intricate design of the bug, showcasing its highly reflective surface and precise construction. Every tiny detail of the subject is carefully captured, from the intricate circuit-like patterns on its body to the sharp edges and sleek contours. This visually captivating representation exudes a sense of precision and modernity, leaving viewers in awe of the technological marvel before them.

**Seed:** 4238506589

**Image Dimensions:** 1024 x 1024   


| Image               | ![00015-4238506589.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00015-4238506589.png) | ![00015-4238506589.png](/stable-diffusion/best-sdxl-models/images/copax/00015-4238506589.png) | ![00015-4238506589.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00015-4238506589.png) | ![00015-4238506589.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00015-4238506589.png) | ![00015-4238506589.png](/stable-diffusion/best-sdxl-models/images/realvis/00015-4238506589.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Space Ark
**Prompt:** A resplendent interstellar ark glimmers with ethereal beauty in this awe-inspiring digital anime image. The ark, glowing with celestial hues, is depicted as a sleek, futuristic spacecraft adorned with intricate patterns reminiscent of constellations. Its elegant design and graceful curves convey a sense of otherworldly enchantment. The scene is captured in a highly detailed photograph, perfectly taken to showcase the intricate interplay of light and shadow. The image invites viewers to embark on a mesmerizing journey through the vast expanse of the cosmos, where the boundaries of imagination and reality blur into one harmonious composition.

**Seed:** 3076404424

**Image Dimensions:** 1024 x 1024   


| Image               | ![00016-3076404424.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00016-3076404424.png) | ![00016-3076404424.png](/stable-diffusion/best-sdxl-models/images/copax/00016-3076404424.png) | ![00016-3076404424.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00016-3076404424.png) | ![00016-3076404424.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00016-3076404424.png) | ![00016-3076404424.png](/stable-diffusion/best-sdxl-models/images/realvis/00016-3076404424.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Bali Waterfall
**Prompt:** In the enchanting landscape of Bali, a magnificent waterfall cascades down with breathtaking force, its power resonating throughout the lush surroundings. This vivid portrayal captures the essence of nature's relentless beauty, whether through a stunning photograph or a meticulously painted masterpiece. The crystal-clear waters, shimmering under the sunlight, evoke a sense of serenity and purity as they plunge into the pool below, creating a captivating symphony of sound and movement. The verdant foliage surrounding the waterfall adds a touch of tranquility, contrasting with the raw energy displayed by the rushing torrent. Each droplet is frozen in time, radiating a vibrant radiance that brings the image to life. This extraordinary portrayal invites viewers to immerse themselves in the sublime grandeur of Bali's natural wonders.

**Seed:** 2597596686

**Image Dimensions:** 1024 x 1024   


| Image               | ![00017-2597596686.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00017-2597596686.png) | ![00017-2597596686.png](/stable-diffusion/best-sdxl-models/images/copax/00017-2597596686.png) | ![00017-2597596686.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00017-2597596686.png) | ![00017-2597596686.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00017-2597596686.png) | ![00017-2597596686.png](/stable-diffusion/best-sdxl-models/images/realvis/00017-2597596686.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Cabin in the Snow
**Prompt:** a beautiful cabin in the snow, light coming out of the windows, cute, cozy atmosphere

**Seed:** 4028737961

**Image Dimensions:** 1024 x 1024   


| Image               | ![00018-4028737961.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00018-4028737961.png) | ![00018-4028737961.png](/stable-diffusion/best-sdxl-models/images/copax/00018-4028737961.png) | ![00018-4028737961.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00018-4028737961.png) | ![00018-4028737961.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00018-4028737961.png) | ![00018-4028737961.png](/stable-diffusion/best-sdxl-models/images/realvis/00018-4028737961.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## AI Dream Sequence
**Prompt:** In a hauntingly surreal AI dream sequence, an enigmatic figure emerges against a backdrop of noir-inspired allure. The vintage photograph captures a woman, dressed in a billowing obsidian gown, her pale skin reminiscent of porcelain. The image is a meticulously crafted, black and white photograph, radiating an air of mystery and sophistication. Delicate strands of pearls drape from her neck, cascading onto her exquisite lace gloves. Her piercing gaze, framed by long lashes, hints at an untold story hidden behind a smokescreen of elegance.

**Seed:** 519653091

**Image Dimensions:** 1024 x 1024   


| Image               | ![00019-519653091.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00019-519653091.png) | ![00019-519653091.png](/stable-diffusion/best-sdxl-models/images/copax/00019-519653091.png) | ![00019-519653091.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00019-519653091.png) | ![00019-519653091.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00019-519653091.png) | ![00019-519653091.png](/stable-diffusion/best-sdxl-models/images/realvis/00019-519653091.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Rainbow Alien
**Prompt:** an exotic but cute alien with multicolored skin and big cute eyes, uhd, 4k, highly detailed

**Seed:** 3723691895

**Image Dimensions:** 1024 x 1024   


| Image               | ![00020-3723691895.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00020-3723691895.png) | ![00020-3723691895.png](/stable-diffusion/best-sdxl-models/images/copax/00020-3723691895.png) | ![00020-3723691895.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00020-3723691895.png) | ![00020-3723691895.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00020-3723691895.png) | ![00020-3723691895.png](/stable-diffusion/best-sdxl-models/images/realvis/00020-3723691895.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Anime Girl
**Prompt:** Highly detailed, High Quality, Masterpiece, beautiful, Nakiri Ayame, long hair, side ponytail, AyameNewYears, red kimono, floral print, hair flower, sash, wide sleeves, white background, scenery, ink, mountains, water, trees, anime style

**Seed:** 248681639

**Image Dimensions:** 1024 x 1024   


| Image               | ![00021-248681639.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00021-248681639.png) | ![00021-248681639.png](/stable-diffusion/best-sdxl-models/images/copax/00021-248681639.png) | ![00021-248681639.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00021-248681639.png) | ![00021-248681639.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00021-248681639.png) | ![00021-248681639.png](/stable-diffusion/best-sdxl-models/images/realvis/00021-248681639.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Robotic Venus
**Prompt:** Roboticizer,Create a hyper-realistic digital painting of the Venus de Milo reimagined as an advanced robot, exuding a dramatic and sorrowful aura. Her robotic form is crafted from high-quality metal with exceptionally detailed engravings and filigree, showcasing an intricate blend of classical artistry and futuristic design. The metal should have a texture similar to aged bronze or weathered silver, adding a historical touch to the robotic figure. Venus's pose is melancholic, with her head gently tilted downwards, suggesting a sense of deep contemplation or lamentation. The robotic face, while retaining the serene beauty of the original sculpture, should have subtle mechanical features that convey a poignant expression. The background is an ethereal, dimly-lit setting, possibly an abandoned classical temple or a futuristic gallery, with dramatic lighting casting stark shadows and highlighting the exquisite details of her metallic body. The overall atmosphere should be one of haunting beauty, blending the sorrowful grace of the ancient world with the solemn elegance of robotic art.  

**Seed:** 4286404194 

**Image Dimensions:** 1024 x 1024   


| Image               | ![00022-4286404194.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00022-4286404194.png) | ![00022-4286404194.png](/stable-diffusion/best-sdxl-models/images/copax/00022-4286404194.png) | ![00022-4286404194.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00022-4286404194.png) | ![00022-4286404194.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00022-4286404194.png) | ![00022-4286404194.png](/stable-diffusion/best-sdxl-models/images/realvis/00022-4286404194.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Macro Rose
**Prompt:** Macro Photography, a rose, shining starlight, Simple background, Dark background, Extreme Detail, UHD,8K, Studio Lighting, Professional Photography, fine art  

**Seed:** 2465035406  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00023-2465035406.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00023-2465035406.png) | ![00023-2465035406.png](/stable-diffusion/best-sdxl-models/images/copax/00023-2465035406.png) | ![00023-2465035406.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00023-2465035406.png) | ![00023-2465035406.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00023-2465035406.png) | ![00023-2465035406.png](/stable-diffusion/best-sdxl-models/images/realvis/00023-2465035406.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |


## Christmas Girl
**Prompt:** (extremely detailed CG unity 8k wallpaper), masterpiece, best quality, 1girl black hair, wearing christmas sweater, christmas decoration in background, lit fireplace in background  

**Seed:** 4289984695  

**Image Dimensions:** 1024 x 1024  


| Image               | ![00024-4289984695.png](/stable-diffusion/best-sdxl-models/images/sdxl-1/00024-4289984695.png) | ![00024-4289984695.png](/stable-diffusion/best-sdxl-models/images/copax/00024-4289984695.png) | ![00024-4289984695.png](/stable-diffusion/best-sdxl-models/images/dreamshaper/00024-4289984695.png) | ![00024-4289984695.png](/stable-diffusion/best-sdxl-models/images/juggernaut/00024-4289984695.png) | ![00024-4289984695.png](/stable-diffusion/best-sdxl-models/images/realvis/00024-4289984695.png) |
|---------------------|--------------------------------------------------------|-----------------------------------------------------|--------------------------------------------------|--------------------------------------------------|-------------------------------------------------|
| Model              | SDXL base 1.0 with 0.9 VAE + SDXL refiner 1.0 with 0.9 VAE | Copax TimeLessXL Version V9                         | Dreamshaper XL v2 Turbo DPMpp SDE                 | Juggernaut XL V8 + RunDiffusion                  | RealVisXL V3.0 (Baked VAE)                      |
| Sampler             | DPM++ 2M Karras        | DPM 3M++ SDE Exponential    |        DPM++ SDE Karras                         |           DPM++ 2M Karras                       |                        DPM++ SDE Karras     | 
| Sampling Steps      | 20                      | 30                          |         6                        |            35                     |                           6  |
| CFG                 | 7                       | 7                           |    2                             |      4.5                           |         2                    |
| Negative Prompt     | None                    | (worst quality, low quality, illustration, 3d, 2d), open mouth, tooth, ugly face, old face, long neck |            None               |              None                   |                          (worst quality, low quality, illustration, 3d, 2d, painting, cartoons, sketch), open mouth   |
