# Step 5 in Building a Prompt Formula:Image Quality

Image quality pertains to the level of detail in a picture. Like many AI image generation tools, including Stable Diffusion, there are distinct parameters that impact quality. Specifically, you can determine the resolution and size of an image by adjusting them. Yet, based on my experience, there are specific "magic words" associated with image quality that can enhance what the AI produces. While these won't affect image size or resolution, they will enhance the visual appeal. 

Our prompt formula now extends to:

```markdown
<Artistic medium> <Adjective> Subject <Action or Accessory> <Location> <Artistic style> <Aesthetics> <Image quality>
```

Some common magic words for image quality are:

- **HD (High Definition)**: Standard resolution for clear and detailed images, often 1920 x 1080 pixels.

- **HDR (High Dynamic Range)**: Enhances contrast and color range for more realistic and vibrant images.

- **UHD (Ultra High Definition)**: Higher resolution than HD, typically at least 3840 x 2160 pixels.

- **4K**: A resolution standard with around 4000 pixels width, offering exceptionally sharp and detailed images.

- **Highly Detailed**: Indicates an image with an abundance of intricate elements and clarity.

- **8K**: Extremely high resolution, around 8000 pixels width, providing exceptional clarity and detail.


## Example: A Landscape

> To demonstrate how image quality influences the picture, I generated two images under identical conditions and using the same seed. The only difference was the incorporation of magic words.

| Prompt | Image | Prompt Breakdown |
| ------------------- | ----- | ------------------ |
| A landscape | ![landscape](/images/prompt-formula/quality/landscape.png) | <ul><li><strong>Subject:</strong> Landscape </li><li><strong>Adjective:</strong> Not specifiec </li><li><strong>Location:</strong> Not specified </li><li><strong>Action or Accessory:</strong> Not specified </li><li><strong>Artistic medium:</strong> Not specified </li><li><strong>Artistic style:</strong> Not specified </li><li><strong>Aesthetics:</strong> Not specified </li><li><strong>Image quality:</strong> Not specified </li></ul> |
| A landscape, 4k, 8k, UHD, highly detailed | ![landscape](/images/prompt-formula/quality/landscape-magic.png) | <ul><li><strong>Subject:</strong> Landscape </li><li><strong>Adjective:</strong> Not specifiec </li><li><strong>Location:</strong> Not specified </li><li><strong>Action or Accessory:</strong> Not specified </li><li><strong>Artistic medium:</strong> Not specified </li><li><strong>Artistic style:</strong> Not specified </li><li><strong>Aesthetics:</strong> Not specified </li><li><strong>Image quality:</strong> 4k, 8k, UHD, highly detailed </li></ul> |

## Examples

| Prompt | Image | Prompt Breakdown |
| ------------------- | ----- | ------------------ |
| Portrait of Morgan Freeman, studio lighting, UHD, highly detailed, HDR | ![Morgan Freeman](/images/prompt-formula/quality/morgan-freeman.png) | <ul><li><strong>Subject:</strong> Morgan Freeman </li><li><strong>Adjective:</strong> Not specified </li><li><strong>Location:</strong> Not specified </li><li><strong>Action or Accessory:</strong> Not specified </li><li><strong>Artistic medium:</strong> Not specified </li><li><strong>Artistic style:</strong> Portrait </li><li><strong>Aesthetics:</strong> Not specified </li><li><strong>Image quality:</strong> UHD, highly detailed, HDR </li></ul> |
| The pyramids of Giza, 4k, 8k | ![Pyramids](/images/prompt-formula/quality/pyramids.png) | <ul><li><strong>Subject:</strong> The pyramids of Giza </li><li><strong>Adjective:</strong> Not specified </li><li><strong>Location:</strong> Not specified </li><li><strong>Action or Accessory:</strong> Not specified </li><li><strong>Artistic medium:</strong> Not specified </li><li><strong>Artistic style:</strong> Not specified </li><li><strong>Aesthetics:</strong> Not specified </li><li><strong>Image quality:</strong> 4k, 8k </li></ul> |
| A female cyborg in space, ultra detailed, 8k, UHD, HDR, HD | ![Cyborg](/images/prompt-formula/quality/cyborg.png) | <ul><li><strong>Subject:</strong> A female cyborg </li><li><strong>Adjective:</strong> Not specified </li><li><strong>Location:</strong> In space </li><li><strong>Action or Accessory:</strong> Not specified </li><li><strong>Artistic medium:</strong> Not specified </li><li><strong>Artistic style:</strong> Not specified </li><li><strong>Aesthetics:</strong> Not specified </li><li><strong>Image quality:</strong> ultra detailed, 8k, UHD, HDR, HD </li></ul> |