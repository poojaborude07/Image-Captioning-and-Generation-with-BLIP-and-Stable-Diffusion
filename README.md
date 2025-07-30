# 🧠📷 Image Captioning + Generation using BLIP and Stable Diffusion

This project demonstrates a **hybrid Generative AI pipeline** that combines two powerful models:

**1. BLIP (Bootstrapping Language-Image Pretraining)**: Automatically generates descriptive captions from input images.

**2. Stable Diffusion**: Uses these captions as prompts to generate new, realistic images — essentially visualizing the text back into images.

The result is a complete **Image → Text → Image** flow using state-of-the-art pre-trained models.

---

## Project Structure
The project is divided into two main blocks:

## 🔹 Block 1: Image Captioning using BLIP
- Upload a folder of images (/content/images) directly from the Colab file explorer.

- BLIP generates captions for each image using a transformer-based encoder-decoder model.

- Captions are printed and displayed alongside the original images.

- You can control the length and quality of the generated text using max_length and num_beams.

## 🔹 Block 2: Image Generation using Stable Diffusion
- Add the captions to a list of prompts.

- Stable Diffusion uses these prompts to synthesize realistic images matching the description.

- Generated images are displayed (or optionally saved/downloaded).

---

## Credits

This project uses the following open-source models:

| Model                                                                         | Purpose                   | Source                    | License                                                                                         |
| ----------------------------------------------------------------------------- | ------------------------- | ------------------------- | ----------------------------------------------------------------------------------------------- |
| [BLIP (base)](https://huggingface.co/Salesforce/blip-image-captioning-base)   | Image → Text (Captioning) | Hugging Face (Salesforce) | [MIT License](https://opensource.org/licenses/MIT)                                              |
| [Stable Diffusion v1.4](https://huggingface.co/CompVis/stable-diffusion-v1-4) | Text → Image (Generation) | Hugging Face (CompVis)    | [CreativeML OpenRAIL-M](https://huggingface.co/CompVis/stable-diffusion-v1-4/blob/main/LICENSE) |

---

## Disclaimer

This project uses the Stable Diffusion v1.4 model, which is released under the [CreativeML OpenRAIL-M License](https://huggingface.co/CompVis/stable-diffusion-v1-4/blob/main/LICENSE). This license permits use, distribution, and modification, provided that the model is not used for harmful or unethical purposes.
