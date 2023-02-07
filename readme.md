# nd_pak.bt
by alphaZomega

This is a template for reading Naughty Dog pak files, specifically for Uncharted 4 on PC.
Support for more games may be added in the future.

# Installation / Usage
1. Download via "Code -> Download as ZIP"
2. Extract
3. In 010 Editor, go to Templates -> View Installed Templates
4. Install the bt file
5. Open any Naughty Dog .pak file with 010 (Some files may require running the template manually
6. Explore pak file contents in page\[0] and page\[1] -> Item


Currently, the following structs are mostly mapped out:
- GEOMETRY_1 (mesh)
- JOINT_HIERARCHY (bones) 
- VRAM_DESC (texture)
- VRAM_DESC_TABLE
- TEXTURE_TABLE

 Other structs contents can be explored only with a generic "Test" scanner.
 
 Inside GEOMETRY_1, you can change material properties such as color and swap materials and their textures by swapping pointers:
 ![params](https://i.imgur.com/lnaCh93.png)
 ![redshirt](https://i.imgur.com/Kwyg327.jpg)
 
 You can also potentially do things like disable extra vertex components that are causing issues with [model editing](https://github.com/alphazolam/fmt_nd_pak)
 
 Thanks to icemesh for the help