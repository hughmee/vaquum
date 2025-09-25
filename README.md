# VAQUUM: Are Vague Quantifiers Grounded in Visual Data?
This repository contains the VAQUUM (**Va**gue **Qu**antifiers with **Hu**man Judgments) dataset from our paper [VAQUUM: Are Vague Quantifiers Grounded in Visual Data?](https://aclanthology.org/2025.findings-acl.619/) (Wong et al., 2025).

## Images
The images that we used for the creation of the VAQUUM dataset are sourced from FSC-147 and TallyQA. In `data/dataset.csv`, the `original_img_id` column refers to the image ID that has been assigned by their respective sources (`fsc` or `tqa`). For example, for the image with `img_name = fsc_1074.jpg`, the unique identifier for this image in the original FSC-147 dataset is `1074`. In this file, you will also find the object of interest (the `object` column) as well as the corresponding object count (`count`) from their sources.

**If any of the links below do not work, please contact their respective authors to obtain access to the datasets.**

### FSC-147
- Link to the original repo: [https://github.com/cvlab-stonybrook/LearningToCountEverything](https://github.com/cvlab-stonybrook/LearningToCountEverything).
- Link to the original images repo: [https://drive.google.com/file/d/1ymDYrGs9DSRicfZbSCDiOu0ikGDh5k6S/view?usp=sharing](https://drive.google.com/file/d/1ymDYrGs9DSRicfZbSCDiOu0ikGDh5k6S/view?usp=sharing)

After downloading, the images are contained in the `images_384_VarV2` folder and are named `XXXX.jpg`, where `XXXX` corresponds to our `orginal_img_id` column.

Note that for the `count` column in our dataset, some values from the FSC-147 ground truths were overwritten by corrected data in the FSC-133 dataset. Image IDs still follow the original FSC-147 dataset as described above.

### TallyQA
- Link to the original repo: [https://github.com/manoja328/TallyQA_dataset](https://github.com/manoja328/TallyQA_dataset)
- Link to the original annotations: [https://github.com/manoja328/tallyqa/blob/master/tallyqa.zip?raw=true](https://github.com/manoja328/tallyqa/blob/master/tallyqa.zip?raw=true)
- Link to the original images repo: [https://homes.cs.washington.edu/~ranjay/visualgenome/api.html](https://homes.cs.washington.edu/~ranjay/visualgenome/api.html)

For TallyQA, we sample images from the **test set** that are classified as `simple` in their metadata. Note that while TallyQA contains images from both COCO and Visual Genome, the test set only contains images from Visual Genome (VG). VG images are contained in a folder with the name `VG_100K_2`. As before, our `original_img_id` column corresponds to the image names.






## BibTex
If you decide to use our dataset, we would appreciate it if you cite our paper.



```bibtex
@inproceedings{wong-etal-2025-vaquum,
    title = "{VAQUUM}: Are Vague Quantifiers Grounded in Visual Data?",
    author = "Wong, Hugh Mee  and Nouwen, Rick and Gatt, Albert",
    editor = "Che, Wanxiang  and Nabende, Joyce  and Shutova, Ekaterina and Pilehvar, Mohammad Taher",
    booktitle = "Findings of the Association for Computational Linguistics: ACL 2025",
    month = jul,
    year = "2025",
    address = "Vienna, Austria",
    publisher = "Association for Computational Linguistics",
    url = "https://aclanthology.org/2025.findings-acl.619/",
    doi = "10.18653/v1/2025.findings-acl.619",
    pages = "11966--11982",
    ISBN = "979-8-89176-256-5"
}
```

## References
Manoj Acharya, Kushal Kafle, and Christopher Kanan. 2019. TallyQA: Answering complex counting questions. In Proceedings of the AAAI conference on artificial intelligence, volume 33, pages 8076–8084.

Michael Hobley and Victor Prisacariu. 2023. Learning to count anything: Reference-less class-agnostic counting with weak supervision. Proceedings of the IEEE Conference on Computer Vision and Pattern Recognition (CVPR).

Viresh Ranjan, Udbhav Sharma, Thu Nguyen, and Minh Hoai. 2021. Learning To Count Everything . In 2021 IEEE/CVF Conference on Computer Vision and Pattern Recognition (CVPR), pages 3393–3402, Los Alamitos, CA, USA. IEEE Computer Society.

Hugh Mee Wong, Rick Nouwen, and Albert Gatt. 2025. VAQUUM: Are Vague Quantifiers Grounded in Visual Data?. In Findings of the Association for Computational Linguistics: ACL 2025, pages 11966–11982, Vienna, Austria. Association for Computational Linguistics.


