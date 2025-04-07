# Introduction to Layered Texturing

PBR Painter uses a layer-based system to allow you to build complex and realistic materials. This system uses Blender's shader nodes under-the-hood, generating complex node setups automatically. However, the general concepts are intuitive and easy to grasp. This documentation explains these concepts, both generally and specific to PBR Painter, to help you understand and utilise the layering system effectively.

The documentation below is intended to get your started with layered texturing, both generally and specific to PBR Painter. Along with the videos, it provides a solid foundation for using PBR Painter. However, it is strongly recommended that you also check out the [hands on tutorails](./hands_on_tutorials.md), which show how to actually apply these concepts to texture your models. 

## General Concepts of Layered Texturing

The video below provides an introduction to layered texturing in PBR Painter and is a great starting point if you are new to the concept:

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/3fmQITzS4Hk?si=QKCeV2xSWBnNh35V" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</p>

Layered texturing is a powerful technique in 3D material creation that allows you to build up complex materials by stacking and blending multiple layers. Each layer can control specific aspects of a material, such as the base material, coatings, imperfections, peeling materials, and more. By separating these properties into layers, you can work on each aspect independently, providing greater flexibility and control.

For example, a base layer might define an underlying metallic material, while additional layers can add details like dirt, scratches, rust or peeling paint. Masks can be applied to layers to control where and how they affect the material, enabling precise customization (more on masks [here.](./layer_masks.md))


### Layer Modes: Filled vs. Painted

Each layer in PBR Painter can be set to one of two modes:

- **Filled Layers**: These layers apply their effects uniformly across the entire material. They are ideal for creating base layers or global effects. Masks can then be added later for further refinement.

- **Painted Layers**: Painted layers include a built-in painted mask that allows you to paint directly onto the material. This is useful as a quick and streamlined workflow for adding localised details or custom hand-painted effects. 

### Channels and Blending

Each layer in PBR Painter can control multiple channels, such as color, metallic, roughness, and normals. Channels can be enabled or disabled individually. Channels are discussed in more detail [here.](./channel_types.md).

### Layer Blending

You can blend layers in all sorts of unique ways, with or without masks. Entire layers, or individual channels, can be blended with underlying layers using various blending modes (e.g., mix, multiply, overlay etc.). 

The most common tools available for blending (outside of masks) are:

- **Opacity**: You can control the overall opacity of a layer or adjust the opacity of individual channels for fine-tuned blending.

- **Normal Blending**: PBR Painter provides a unique "Combine Normals" feature that mathematically blends normal maps across layers for accurate results. You can also control the strength of underlying normals to achieve specific effects.

### Layer Bumping

PBR Painter includes streamlined layer bumping, which allows you to offset an entire layer's surface to create raised or recessed effects. This is particularly useful for adding details like engravings or embossed patterns.

## Layer Types in PBR Painter

The video below provides a detailed explanation of the specific layer types used in PBR Painter and how to use them effectively:

<p>
<iframe width="560" height="315" src="https://www.youtube.com/embed/krhDbO6nSRU?si=ipNtODiB_JI_J7WG" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
</p>

PBR Painter offers three main types of layers, each designed for specific use cases. These are discussed briefly here then in more detail later in this documentation. The layer types are:

1. **Standard Layers**:  
   These are the most commonly used layers in PBR Painter. They provide a user-friendly interface for controlling material properties such as color, metallic, roughness, and more. Standard layers are designed to work seamlessly with the PBR Painter UI, allowing you to make adjustments without needing to interact directly with the underlying node setup.

2. **Custom Nodes Layers**:  
   Custom nodes layers allow advanced users to break out of the constraints of the standard layer system and create entirely custom node setups. These layers still integrate with PBR Painter's masking system, enabling you to combine custom node setups with procedural or painted masks.

3. **Multipaint Layers**:  
   Multipaint layers are a powerful feature introduced in PBR Painter 3. They allow you to project complex PBR materials (e.g., base color, metallic, roughness, etc.) onto your model simultaneously. This is particularly useful for painting decals or covering seams in your materials.

### Practical Workflow in PBR Painter

To create a material in PBR Painter, follow these general steps:

1. **Set Up the Material**:  
   Begin by setting up your material in PBR Painter. You can choose to use an existing material as a background or start with a new one.

2. **Add Layers**:  
   Add layers to define different aspects of your material. For example, start with a base metallic material, then add layers for details like scratches, dirt, or metallic highlights.

3. **Apply Masks**:  
   Use masks to control where each layer is applied. Experiment with procedural masks, painted masks, or a combination of both.

4. **Adjust Blending**:  
   Fine-tune the blending modes and opacity settings for each layer to achieve the desired look.

5. **Preview and Refine**:  
   Use PBR Painter's real-time preview capabilities to see how your material looks and make adjustments as needed.

## Conclusion

The layering system in PBR Painter is a powerful tool for creating complex and realistic materials. By understanding the general concepts of layered texturing and the specific features of PBR Painter, you can unlock the full potential of this system and create stunning 3D materials with ease. Experiment with different layer types, masks, and blending modes to discover the possibilities and refine your workflow.