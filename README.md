Get start
======


Once again, we did a lot of work on the basis, transforming the single-modal model into a text-led multi-modal model,
building our own dataset, expanding the research object under multi-task, multi-scenario and multi-climate conditions, and extending the research problems to disaster assessment,
crop yield prediction and sea level supervision.
Solving three difficultity in building change detection,for example:
<img width="800" height="550" alt="image" src="https://github.com/user-attachments/assets/31ab86f4-449b-43be-b8bb-a85d7692bb11" />


Next I will explain the contents of TMCD:

<img width="700" height="800" alt="image" src="https://github.com/user-attachments/assets/1406152a-a7c7-4dfe-8fe7-d7fdc1794715" />

As shown in the schematic above, our change detection framework is based on text and image expansion, and features are aggregated by image encoder GDC and text encoder TGL.

<img width="566" height="650" alt="image" src="https://github.com/user-attachments/assets/b097250d-638d-4833-97b0-9652b924fcdd" />

Different from other networks, here we mainly study the multi-task detection (including changes in buildings, farmland, and water) under dark fog conditions, as shown above.


How to use
------
Models
*resnet50
*resnet34

Environment
---------
![1](https://github.com/user-attachments/assets/00c94add-a4fc-4e65-b7c6-caead64d87e0)

![2](https://github.com/user-attachments/assets/d6408a2b-e7d3-40c9-ac15-8d0c4ab8a216)

Datasets processing
------
We generate a new Levi-NC, SYSU-NC, CCLD-NC dataset on the Levi-cd, CCLD,Sysu-cd dataset。
The detailed conversion code is exposed in the main function.

Dataset 
---
You should set your own path in the dataset.

Train
----
multi-modal train.py

Save model
---
We save the model in pth format and also upload it to the main function.

Test
---
Changing the path of the trained model (pth) in output2.py will generate the visual results of the test and save them in the set path.



License
===
All images and codes in TMCD can be used for academic purposes only, but any commercial use is prohibited.
**All codes will be provided after the paper is accepted**


