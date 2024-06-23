# Step 1 in Building a Prompt Formula: The Subject

The subject is what you want to see in the generated image. Ask yourself: do I want an image of a person? An animal or perhaps a landscape? 

For instance, let's focus on a cat as our subject.

Then, we need to consider the following questions:
- How do you characterize the cat? For instance, is the cat "adorable"?
- Are there particular characteristics you want for the cat? For example, the cat has "black fur and blue eyes."
- Where can the cat be found? For instance, "the cat is resting on a table."
- Are there any additional items the cat should have? For example, the cat is "wearing a red collar."

These questions collectively result in the following prompt formula:

```markdown
<Adjective> Subject <Action or Accessory> <Location>
```

- **Subject**: This is the central element you're addressing or emphasizing in your description. The subject can encompass a wide range of things, such as people, animals, objects, locations, plants, vehicles, food, weather conditions, natural occurrences, and abstract ideas.  It's the only mandatory part of the formula, so you must include it.
- **Adjective (Optional)**: You can use an adjective to add a descriptive word that helps paint a clearer picture of the subject. Adjectives can come before or after the Subject. This means you can use descriptive words to talk about the Subject, and you have the flexibility to place them before or after the main focus of your image.
- **Action or Accessory (Optional)**: This is where you can include an action or an item that's related to the subject, but it's not required.
- **Location (Optional)**: If you want to specify where the scene takes place, you can use this element. However, it's also optional.

## Examples


| Prompt | Image | Prompt Breakdown |
| ------------------- | ----- | ------------------ |
| A cute black cat with blue eyes wearing a red collar lying on a table | ![cute-black-cat](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/cute-black-cat.png) | <ul><li><strong>Subject:</strong> cat</li><li><strong>Adjective:</strong> cute, black, with blue eyes</li><li><strong>Location:</strong> lying on a table</li><li><strong>Action or Accessory:</strong> wearing a red collar</li></ul> |
| A cheerful young woman with long, curly hair holding a bouquet of colorful flowers in a garden | ![cheeerful young woman in garden](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/cheerful-young-woman-in-garden.png) | <ul><li><strong>Subject:</strong> woman</li><li><strong>Adjective:</strong> cheerful, young, with long curly hair</li><li><strong>Location:</strong> in a garden</li><li><strong>Action or Accessory:</strong> holding a bouquet of colorful flowers</li></ul> |
| Enchanted forest with ancient trees | ![enchanted forest](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/enchanted-forest.png) | <ul><li><strong>Subject:</strong> Forest</li><li><strong>Adjective:</strong> Enchanted</li><li><strong>Location:</strong> Not specified</li><li><strong>Action or Accessory:</strong> Ancient trees</li></ul> |
| A curious cat exploring a mysterious cardboard box | ![cat in cardbox](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/cat-in-cardbox.png) | <ul><li><strong>Subject:</strong> Cat</li><li><strong>Adjective:</strong> Curious</li><li><strong>Location:</strong> Not specified</li><li><strong>Action or Accessory:</strong> Exploring a mysterious cardboard box</li></ul> |
| Delicious pizza at a cozy Italian restaurant | ![pizza in restaurant](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/pizza-in-restaurant.png) | <ul><li><strong>Subject:</strong> Pizza</li><li><strong>Adjective:</strong> Delicious</li><li><strong>Location:</strong> Cozy Italian restaurant</li><li><strong>Action or Accessory:</strong> Not specified</li></ul> |
| Sparkling stars in the dark night sky | ![stars in night sky](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/stars-in-night-sky.png) | <ul><li><strong>Subject:</strong> Stars</li><li><strong>Adjective:</strong> Sparkling</li><li><strong>Location:</strong> Dark night sky</li><li><strong>Action or Accessory:</strong> Not specified</li></ul> |
| Tranquil waves lapping the sandy beach | ![waves on beach](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/waves-on-beach.png) | <ul><li><strong>Subject:</strong> Waves</li><li><strong>Adjective:</strong> Tranquil</li><li><strong>Location:</strong> Not specified</li><li><strong>Action or Accessory:</strong> Lapping the sandy beach</li></ul> |
| Joyful children playing with colorful balloons in the park | ![children playing](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/children-playing.png) | <ul><li><strong>Subject:</strong> Children</li><li><strong>Adjective:</strong> Joyful</li><li><strong>Location:</strong> Park</li><li><strong>Action or Accessory:</strong> Playing with colorful balloons</li></ul> |
| Racing down the winding mountain road, a sleek sports car | ![sports car](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/sports-car.png) | <ul><li><strong>Subject:</strong> Sports car</li><li><strong>Adjective:</strong> Sleek</li><li><strong>Location:</strong> Not specified</li><li><strong>Action or Accessory:</strong> Racing down the winding mountain road</li></ul> |
| An Owl | ![owl](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/owl.png) | <ul><li><strong>Subject:</strong> Owl</li><li><strong>Adjective:</strong> Not specified</li><li><strong>Location:</strong> Not specified</li><li><strong>Action or Accessory:</strong> Not specified</li></ul> |
| Busy city street, filled with rushing commuters | ![busy city](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/subject/city-with-commuters.png) | <ul><li><strong>Subject:</strong> City street</li><li><strong>Adjective:</strong> Busy</li><li><strong>Location:</strong> Not specified</li><li><strong>Action or Accessory:</strong> Filled with rushing commuters</li></ul> |