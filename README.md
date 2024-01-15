# Visual Grounding

Borghini Alessia (1834906), Di Valerio Federico (1835405)

**Visual Grounding** (VG) is the task of locating an object instance from an image referred by a query sentence. VG is a multimodal task that requires the machine to understand the complex reasoning in the textual query, as well as the spatial and semantic relationships among the instances in the image.

![image](https://github.com/ABorghini/VP_Visual_Grounding/assets/80713403/3f1765ca-8be1-4d54-873e-dc1b78041928)

The general workflow of the algorithms we compared in this project are listed here:
- **Baseline model**: extract the descriptions of the objects in the image and compare such descriptions with the query in order to obtain the best matching bounding box;
![baseline](https://github.com/ABorghini/VP_Visual_Grounding/assets/80713403/9d376b2b-b72d-4e16-b1f3-49d07e6f622f)

- **Clip model**: we used the clip model in order to obtain embeddings of images and texts in the same space;
![clip](https://github.com/ABorghini/VP_Visual_Grounding/assets/80713403/5cc450cf-cf12-4088-9dc7-10840a85f7a0)

- **Clip with heatmaps**: we exploited the use of the explainability nature of clip in order to find the object that mostly activated the clip model when also the query is fed to it. 
![clip_heat](https://github.com/ABorghini/VP_Visual_Grounding/assets/80713403/f5d3853f-0cb5-4e1f-9620-d1ebf118a83d)
