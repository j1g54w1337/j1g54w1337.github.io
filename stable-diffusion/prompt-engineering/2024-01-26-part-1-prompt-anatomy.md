---
layout: page
title: Chapter 1 - Prompt Anatomy
subtitle: Stable Diffusion Prompt Engineering
cover-img: /assets/img/j1g54w-blog.jpg
thumbnail-img: /assets/img/stable-diffusion/prompt-engineering/elsa-thumb.png
share-img: /assets/img/j1g54w-blog.jpg
tags: [genai, ai, image-generator, new-tech]
---

# Chapter 1 - Anatomy of the prompt
## Where to begin
### Setup point
To start with a new generation you have to setup the basics first. What I always do is choosing the model I like and leave the rest alone, for now. I really love the results of the model **RevAnimated**, so that's also the one I use for this post to start with.

### Hardware setup
* 18 Solar Panels
* Nvidia GeForce GTX 1080Ti
* Nvidia GeForce RTX 3060

### Used sources
* [AI Eenthusiastic - Stable Diffusion Lighting Guide/](https://aienthusiastic.com/stable-diffusion-lighting-guide/)

## Prompt anatomy
A prompt can make you a great image, but a single typo or wrong placement of a word can messup your whole creation and results in a **gompie**. Prompts can be really complex and confusing so it's important to know how the prompt works and how you can build one. Let me take you to a proven prompt anatomy and beaking up each part to explain what it does **"add source of prompt anatomy"**

### The flow
A prompt flow looks like this: **Subject (required) -> Medium -> Style -> Artist -> Website -> Resolution -> Additional details -> Color -> Lighting**

Later I will add examples on each step of the flow, but first I'm going to tell you what each step in the flow means and what it does.

**Subject** - What do you want to generate?
| keyword	| Note |
|:--------|:-----|
| Elsa from Frozen	| This is what your artwork needs to look like |

**Medium** - Define a category of your artwork, below you have some examples of which you can use. 
| keyword	| Note |
|:--------|:-----|
| Portrait	| Very realistic drawings. Good to use with people.|
| Digital painting |	Digital art style.|
| Concept art	| Illustration style, 2D. |
| Ultra realistic illustration |	Drawings that are very realistic. Good to use with people. |
| Underwater portrait	| Use with people. Underwater. Hair floating. |
| Underwater steampunk	| Very realistic drawings. Good to use with people. |

**Style** - Define the style of your artwork
| keyword	| Note |
|:--------|:-----|
| hyperrealistic | Increases details and resolution |
| pop-art	| Pop-art style |
| Modernist | Vibrant color, high contrast |
| art nouveau |	Add ornaments and details, building style |

**Artist** - Add the style of a specific artist
Mentioning the artist in the prompt is a strong effect. Study their work and choose wisely.

| keyword	| Note |
|:--------|:-----|
| John Collier	| 19th century portrait painter. Add elegancy |
| Stanley Artgerm Lau	| Good to use with woman portrait, generate 19th delicate clothing, some impressionism |
| Frida Kahlo	| Quite strong effect following Kahlo’s portrait style. Sometimes result in picture frame |
| John Singer Sargent	| Good to use with woman portraits, generate 19th delicate clothing, some impressionism |
| Alphonse Mucha	| 2D portrait painting in style of Alphonse Mucha |

**Website** - Mentioning an art or photo site is a **strong effect**, probably because each site has its niche genre.
| keyword	| Note |
|:--------|:-----|
| pixiv	| Japanese anime style |
| pixabay	| Commercial stock photo style |
| artstation	| Modern illustration, fantasy |

**Resolution** - Improving the quality of the artwork results
| keyword	| Note |
|:--------|:-----|
| unreal engine	| Very realistic and detailed 3D |
| sharp focus	| Increase resolution |
| 8k	 | Increase resolution, though can lead to it looking more fake. Makes the image more camera like and realistic |
| vray	| 3D rendering best for objects, landscape and building. |

**Additional details** - Add specific details to your image
| keyword	| Note |
|:--------|:-----|
| dramatic	| shot from a low angle |
| silk	| Add silk to clothing |
| expansive	| More open background, smaller subject |
| low angle shot	| shot from low angle |
| god rays	| sunlight breaking through the cloud |
| psychedelic	| vivid color with distortion |

**Color** - Add an additional color scheme to the image.
| keyword	| Note |
|:--------|:-----|
| iridescent gold |	Shinny gold |
| silver	| Silver color |
| vintage	| vintage effect |

**Lightning** - Add specific lightning effects on your artwork
| keyword | Note |
|:--------|:-----|
| Volumetric | Referencing to the presence of visible rays or beams of light in a space |
| Rim lighting | It is a technique where the subject is illuminated from behind, creating a bright outline around the edges of the subject |
| Golden hour | It is the period shortly after sunrise or before sunset when the sunlight is softer, warmer, and diffused |
| Blue hour | It is the period just before sunrise or after sunset when the sky has a deep blue hue |
| Sunlight | It helps to direct light emitted by the sun |
| Dimly light | Create a moody or mysterious atmosphere |
| Broad Lighting | Illuminates the side of the face that is turned towards the camera, making it appear broader |
| Loop Lighting | Creates a small shadow of the nose on the cheek, forming a loop-like shape on the shadowed side of the face |
| Rembrandt Lighting | Named after the famous painter, this technique creates a small triangle of light on the shadowed side of the face, below the eye |
| Butterfly Lighting | Produces a small, butterfly-shaped shadow just below the nose |

## Time to generate some artwork
### Setup your starting point
* Model: RevAnimated
* Steps: 20
* CFG: 7
* Sampler: DPM++ 2M Karras

#### 1. Subject - Generate a couple of images
With a random seed **-1** enabled you generate a couple of images, for this example I create **6 images** with only a subject in the prompt; **Elas from Frozen**

Your prompt looks like this: **Elsa from Frozen**

![c1ec1bae79b059a64b4ec584805d6411.png](../../assets/img/stable-diffusion/prompt-engineeringe9cc56c065a947dd96d78367a94547a7)

Quite impressive already, don't you think? But we can do a lot of improvements by adding more details. Choose the image you like the most and take the **seed** of this image. I go for the top middle one with seed: **438922630**

#### 2. Medium - What category is used for you artwork
This part can be a bit confusing since we put the **medium** in front of the **subject**, but when you read your prompt you'll probably understand why that is. Lets go for: **Ultra realistic illustration** and we generate 6 new images but now with the choosen seed as starting point.

Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen**

![0e16786b14ff2d0eecd988546479f048.png](../../assets/img/stable-diffusion/prompt-engineeringa080abd74e714fdeaa5442b183682ac2)

As you will notice the results are more similar which is a result of using the same seed for all generated images.

#### 3. Style - Adding some style
Now I will generate a couple of examples without changing the settings, I will only change the **style** in the prompt so you can see what it does. It's possible that the results will not be 100% similar, this has to do with the changed prompt that will have influence on the calculations and results.

**1. hyperrealistic**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, hyperrealistic**
![4897af50d920d60dfc4801b26836b304.png](../../assets/img/stable-diffusion/prompt-engineering65ba543a72c949ef989205b949d88107)

**2. pop-art** 
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, pop-art**
![3195d592fc87306de4697f2a97681487.png](../../assets/img/stable-diffusion/prompt-engineering3d498b1145d248f485a662a23f8ad076)

**3. Modernist**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist**
![060ae764ec8748ee1b5e9c77044e6877.png](../../assets/img/stable-diffusion/prompt-engineeringf9a4d1922ca849bbb04ff6b4b19b620d)

**4. art nouveau**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, art nouveau**
![a6362082c7b8a8f5e10a669881e0c5bf.png](../../assets/img/stable-diffusion/prompt-engineering8f42340664a14dbb9d4413ae5674ef47)

I like **Modernist** the most, so I'll pick that one for the rest of the post!

#### 4. Artist - Adding an Artist
When you add an artist to your prompt the AI will create an artwork in the artst style, for example thinking of Van Gogh, or Rembrandt, or combine both to make unique artworks based on the combined styles. Since that approach can also completely mess up your results I will leave that part for you own **trial-and-error** Friday evening. :)

**1. John Collier**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by John Collier**
![fd15d802486c43711292547a26a96f4d.png](../../assets/img/stable-diffusion/prompt-engineering2c34e105ccac4a41aa184a3db58d55db)

In the first creation I've used "by John Collier" but you can also use a **comma seperated** approach which results in something totally different, up to you what you like most!
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist, John Collier**
![eccf17741283a6e0bf40ac94b35d3f35.png](../../assets/img/stable-diffusion/prompt-engineering559aa77f1c39416aa1aa3997823de801)

**2. Stanley Artgerm Lau**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau**
![56ad84af74bbfeb0d083ad0f928450b0.png](../../assets/img/stable-diffusion/prompt-engineeringbfd0d507e6934220bff0e6f4c8d36116)

Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist, Stanley Artgerm Lau**
![7bc7aabe33314fcc8a155aa5d2c4392a.png](../../assets/img/stable-diffusion/prompt-engineering01cfe02875d24c6d9e003261affe9058)

As you can see in this example, the two different prompts will not always lead to completely different creations.

**3. Frida Kahlo**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Frida Kahlo**
![5c7420b7a4c4cb40ee3c61030cb76311.png](../../assets/img/stable-diffusion/prompt-engineering2bc590368da34365b49050379721a37c)

Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist, Frida Kahlo**
![f3053e2ad9f07531ab82b1b41514eec2.png](../../assets/img/stable-diffusion/prompt-engineeringe41100882a034dec83f0a9f934fb02c5)

**4. John Singer Sargent**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by John Singer Sargent**
![9060075168fa3fe75f172d668d72b723.png](../../assets/img/stable-diffusion/prompt-engineeringc657c1d99b2d4e39bf6065ed6ef9cc0a)

Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist, John Singer Sargent**
![9351a16123fd3f91430d278b98ab1202.png](../../assets/img/stable-diffusion/prompt-engineeringc78d1a12e3004e4c93a0a2acdde2ae85)

**5. Alphonse Mucha**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Alphonse Mucha**
![304dee00e25aa62a9c2afb560998fa43.png](../../assets/img/stable-diffusion/prompt-engineering10053720de964f819753a1fec32bc031)

Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist, Alphonse Mucha**
![63ea5ed1bb51a845451aa3b0f3e66eb1.png](../../assets/img/stable-diffusion/prompt-engineering9d1eba31e7914b248dcd2bbdbf362266)

I like the first run from **Stanley Artgerm Lau** the most, so I will continiue with this prompt **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau**

#### 5. Website - Adding a art website as a reference
**1. pixiv**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, pixiv**
![f463d04bc1f824748194325fbd2447ea.png](../../assets/img/stable-diffusion/prompt-engineering90b59418317d4b019f88a822fe494de3)

**2. pixabay**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, pixabay**
![4e533a15815e47586d409749e7bdfd88.png](../../assets/img/stable-diffusion/prompt-engineering38dbd4d1204d4ac4a6ac95997e3a2017)

**3. artstation**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation**
![966e4c0e4ad6d30c799e8b6272ab6f12.png](../../assets/img/stable-diffusion/prompt-engineering27116e197c5e45918bf58832f38cbfd9)

#### 6. Resolution - Improving the quality of the generated results
**1. unreal engine**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, unreal engine**
![38cb25cd06977739d870283b9d92614e.png](../../assets/img/stable-diffusion/prompt-engineering6910fb6047e649c382ad34f7ef429ab9)

**2. sharp focus**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, sharp focus**
![6a2fe7f40403c6a8d105d6e3407d5eeb.png](../../assets/img/stable-diffusion/prompt-engineeringe95cf78f41064d11b571904194ed1594)

**3. 8k**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k**
![ffb97313bb9b88a2e7a4800577a8d956.png](../../assets/img/stable-diffusion/prompt-engineeringdcc1dc0bb8ff47b2a66979ce0c4ef786)

#### 6. Additional details
**1. dramatic**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, dramatic**
![a2ca2af7b93b2c8735ef6e987f0eb215.png](../../assets/img/stable-diffusion/prompt-engineeringd33736c70a7245d6ab647af69ce270fa)

**2. silk**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, silk**
![12f6d3adeb81179b1c4544690a30c452.png](../../assets/img/stable-diffusion/prompt-engineeringa1774defd6b547b798bf50451b70190e)

**3. expansive**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, expansive**
![62a2f7f7cab7ed6fcd0ff6b4fda5e331.png](../../assets/img/stable-diffusion/prompt-engineering2311f431d84d4636b23b0b34c4af5298)

**4. low angle shot**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, low angle shot**
![7ff502161fce20e918c235a562f5f0b0.png](../../assets/img/stable-diffusion/prompt-engineering395cd81020e14e88a3251da96b9ff17b)

**5. god rays**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays**
![ce613da064c8b09f8f3b435e67fd5008.png](../../assets/img/stable-diffusion/prompt-engineering9d54a47e9e9545ffb49f088dc4d1634c)

**6. psychedelic**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, psychedelic**
![0b83123a2302f4a374cb8d63d0adaff0.png](../../assets/img/stable-diffusion/prompt-engineering64b098893e664ee39d970be82e096916)

#### 7. Colors - Adding an additional color scheme to you artwork
**1. iridescent gold**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, iridescent gold**
![16404324f2f2ba34e816e86c82cb73c9.png](../../assets/img/stable-diffusion/prompt-engineering26e0214ad5d8442aa2eec6e50ff0fa2f)

**2. silver**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver**
![e29489fd40ea7a2b4863a79570734253.png](../../assets/img/stable-diffusion/prompt-engineeringc7e884f3bd56496aadd7730b83d19ce0)

**3. vintage**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, vintage**
![16b15a7c0563839e97c0e6db80ee64b1.png](../../assets/img/stable-diffusion/prompt-engineeringe20af07132804ba69ffa98449198e90f)

#### 8. Lightning - Add lightning effects to your artwork
**1. volumetric**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, volumetric**
![a73815209883ba1265d397afa0bc5768.png](../../assets/img/stable-diffusion/prompt-engineering690f75a622364485aad8f842de3bf2e6)

**2. rim lighting**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, rim lighting**
![1b7e8829fd6d06290f018f64f3d44981.png](../../assets/img/stable-diffusion/prompt-engineeringde3b93b00f5e4eaeb6e843df20e182ed)

**3. golden hour**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, golden hour**
![d6b91da7cee9106c17d8a33a5db15361.png](../../assets/img/stable-diffusion/prompt-engineering546ab781befa43cfb612014c9dde78a6)

**4. blue hour**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, blue hour**
![9087872940603c65481167f44caa6ca4.png](../../assets/img/stable-diffusion/prompt-engineering3f69ca157c61451da64e0d87202495f1)

**5. sunlight**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, sunlight**
![00628931b5f6753a09a99a0cc5a3c34a.png](../../assets/img/stable-diffusion/prompt-engineeringc811fb61a48445da8f1d444e8f94a5cb)

**6. dimly light**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, dimly light**
![a5511862f9de5fddc757545a7ce83dc3.png](../../assets/img/stable-diffusion/prompt-engineering5563925bf819490895762c868352e1a6)

**7. broad lightning**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, broad lightning**
![42e30883fe3b71f751b51f4b9509aaf3.png](../../assets/img/stable-diffusion/prompt-engineeringd2ed904a85cd4ab7bd5d33d940caae35)

**8. loop lightning**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, loop lightning**
![864f75de7890bd907cac26a169bb79c4.png](../../assets/img/stable-diffusion/prompt-engineering8cbd6e8e00084203bd588f82354cef98)

**9. rembrandt lightning**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, rembrandt light style, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver**
![f47fe824096c1f2513b96039e11faa68.png](../../assets/img/stable-diffusion/prompt-engineeringf902aeb3aa91452da3b9d38436ef48c1)

**10. butterfly lightning**
Your prompt looks like this: **Ultra realistic illustration of Elsa from Frozen, Modernist by Stanley Artgerm Lau, artstation, 8k, god rays, silver, butterfly lightning**
![a5f27b9eb9c873ae0673c1fd04d40194.png](../../assets/img/stable-diffusion/prompt-engineeringfdc3e223ef4b46fbbe299f6396aa8df2)


