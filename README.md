# Image Processing and Generation Project

This project combines background removal, image inpainting, and scene generation using deep learning techniques. It takes an input image, removes its background, and then generates a new scene based on a text prompt.

## Features

- Background removal from input images
- Mask creation for inpainting
- Scene generation using Stable Diffusion
- Visualization of intermediate steps

## Requirements

- Python 3.7+
- PyTorch
- diffusers
- Pillow
- rembg
- matplotlib
- numpy


## Usage

1. Place your input image in the project directory or update the `image_path` variable in the script with the correct path to your image.

2. Update the `text_prompt` variable with your desired scene description.

3. Run the script: in jupyter notebook


4. The script will generate several output files:
   - `original_image.png`: The original input image
   - `no_background_image.png`: The input image with the background removed
   - `mask_image.png`: The mask used for inpainting
   - `generated_image.png`: The final generated image

## How it Works

1. **Image Loading**: The script loads the input image using Pillow.

2. **Background Removal**: The `rembg` library is used to remove the background from the input image.

3. **Mask Creation**: A mask is created from the alpha channel of the background-removed image.

4. **Image Preprocessing**: The image is resized and centered on a transparent background to fit the required input size for the Stable Diffusion model.

5. **Scene Generation**: The Stable Diffusion Inpainting model is used to generate a new scene based on the text prompt, using the preprocessed image and mask.

6. **Visualization**: Matplotlib is used to display the original image, background-removed image, mask, and the final generated image.
   
SCREENSHOTS
![1](https://github.com/user-attachments/assets/80943ca2-8e68-4eaf-bfa5-d51dd38bcb45)
[2](https://github.com/user-attachments/assets/2451921a-7737-4903-8081-b92f8c874f91)
!![3](https://github.com/user-attachments/assets/051b5df6-7210-436c-b1e2-36c526b9834f)



I have made this part of the assignment using ChatGPT and ClaudeAI 
I tried the video processing one but could not do it was facing many errors
