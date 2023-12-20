# Ink-To-Tint: Manga Artisan

## Motivation

The manga industry often grapples with the intensive labor involved in the creation process, commonly resulting in overworked artists. The meticulous nature of manga drawing typically results in publications featuring black-and-white illustrations. This choice, while traditional, can diminish the reader’s engagement, particularly when an anime adaptation is not yet available. Moreover, while certain art styles are favored, it can be excessively demanding and redundant for artists to reinterpret a series into another style. The implementation of automation through conditional Generative Adversarial Networks (cGANs) for colorization and style transfer via Stable Diffusion model offers a solution. This innovation promises to alleviate the artists’ burden while simultaneously broadening the appeal to diverse audiences, potentially increasing readership and expanding the market. Our initiative aims to foster a greater appreciation of manga as an art form across a wider audience.

## Image Preprocessing

While automatic colorization using cGANs has been successfully implemented in previous studies, these implementations often fall short in authentically replicating the actual manga dataset. Typically, textured and grayscale inputs were employed, resulting in idealistic outputs and an ease of achievement that does not accurately reflect authentic manga styles. To address this gap, our report demonstrates the conversion of a colored manga dataset to its sketched version using image processing techniques such as dodging and dilation.

![image](https://github.com/Anannyap7/ink_to_tint-manga_artisan/assets/59221653/8b57f929-9bf9-4b72-bdba-731b362483ed)

The figure above demonstrates the use of **dodging and dilation** on grayscaled version of the colored input image to obtain the desired dataset.

## Colorization Results

**Model Used:** Pix2Pix condition GAN with residual connections to retain the original input integrity (texts and edges)

The figure below illustrates a marked progression in the quality of colorization with each successive interval of 20 epochs for a total of 80 epochs. Notably, the phenomenon of color spillage observed in the initial stages diminishes over time, and the hues associated with the characters exhibit a dis- cernible deepening in intensity.

![image](https://github.com/Anannyap7/ink_to_tint-manga_artisan/assets/59221653/ebf7b408-e2a5-474b-9db6-65afa1487e77)

Furthermore, the application of our model to unseen data yields commendable results, as evidenced by the vivid and accurate colorization. This outcome is indicative of the model’s robust ability to generalize effectively to novel manga pages.

![image](https://github.com/Anannyap7/ink_to_tint-manga_artisan/assets/59221653/eefa1956-b6b2-46b3-a810-d250f2eacfc1)

## Style Transfer Results

The experimental phase of our study on style transfer was undertaken utilizing a constrained dataset over a finite duration. Preliminary outcomes, as depicted below,
though somewhat irregular in nature, offer a glimpse of the potential advancements achievable in future endeavors. With an expanded dataset and enhanced fine-tuning pro- cesses, these initial results suggest promising directions for further refinement and development in the field of manga style transfer.

![image](https://github.com/Anannyap7/ink_to_tint-manga_artisan/assets/59221653/cdb36282-d220-48f6-bdf7-4a6dd9e3a781)
