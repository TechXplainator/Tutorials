# Prompt Editing

Prompt editing allows you to start sampling one picture, but in the middle swap to something else. 

## Switch Phrases after X Steps

The base syntax is:

```markdown
[phrase1:phrase2:X]
```
X is a number indicating at which step to switch during the sampling cycle. The higher this number, the later the switch happens, and the model has less power to replace phrase1 with phrase2. 

**Example**: 

```markdown
a portrait of [Johnny Depp:Idris Elba:16]
``````
![Elba-Johnny](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/prompt-editing/Elba-Depp.jpeg)

At start, the model will be drawing a portrait of Johnny Depp.
After step 16, it will switch to drawing a portrait of Idris Elba, continuing from where it stopped with Johnny Depp.

## Add Phrase after X Steps

The base syntax is:
```markdown
[phrase:X]
```

**Example**: 

```markdown
A fantasy landscape [with a lake:15]
``````
![mountain-lake](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/prompt-editing/mountain-lake.jpeg)

At start, the model will be generating a fantasy landscape. After step 15, it will switch to generating a fantasy landscape with a lake, but continuing where it stopped with fantasy landscape without the lake. 

## Remove Phrase after X Steps

The base syntax is:
```markdown
[phrase::X]
```

**Example**: 

```markdown
A bar [with red neon light::9]
``````
![bar](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/prompt-editing/bar.png)

At first, Stable Diffusion will generate an image of a bar with red neon light. After 12 steps, it will switch to create an image of a bar, but based on the image of a bar with red neon light.


## Alternate Beteween Phrases
The base syntax is:
```markdown
[phrase1|phrase2]
```
**Example**: 

```markdown
A [pig|monkey] in a barn
``````
![pig-monkey](/stable-diffusion/write-better-prompts-for-stable-diffusion/images/prompt-editing/pig-monkey.png)

Stable Diffusion switches back and forth between creating an image of a pig in a barn and a monkey in a barn in each step.

You can expand this syntax to more than 2 phrases. In that case, Stable Diffusion will cycle through phrases 1, 2, up to N, and then loop back to phrase 1:

```markdown
[phrase1|phrase2|...|phraseN] - alternates between phrase1 ... phraseN, then loops back to phrase1
```