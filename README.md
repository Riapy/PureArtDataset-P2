# 🖼️ P2: A Purified Style Classification Dataset

This repository provides the **P2 dataset**, a curated and purified image dataset for evaluating **style classification models** in the context of **artistic image analysis**. It was constructed as part of our paper:

```
bibtex
/
```



## 📁 Dataset Overview

P2 is a purified version of existing style classification datasets (Painting91, Pandora, WikiArt3), created by filtering high-uncertainty samples using our proposed **style uncertainty measure** in our paper. The goal is to retain images with **clear and consistent stylistic characteristics**, which significantly improves downstream classification performance.

- **Classes**: 6 style categories (e.g., Abstract-expressionism, Baroque, Impressionism, etc.)
- **Format**: JPEG images organized by class folder
- **Size**: 25710 images
- **Resolution**: Various (recommended resize to 224x224 during training)

| ID   | style                  | P2    |
| :--- | :--------------------- | :---- |
| 1    | Abstract-expressionism | 2972  |
| 2    | Baroque                | 1057  |
| 3    | Impressionism          | 6277  |
| 4    | Realism                | 5622  |
| 5    | Romanticism            | 5276  |
| 6    | Surrealism             | 4509  |
|      | total                  | 25710 |



## 📦 Structure

```
P2/
│
├── Abstract-expressionism/
│   ├── image001.jpg
│   ├── image002.jpg
│   └── ...
├── Baroque/
├── Impressionism/
└── ...
```



## 🖼️ Example Visualization

Below are example images from several style categories in the **P2 dataset**. 

 

| **style**              | **imges**                                                    |                                                              |
| :--------------------- | :----------------------------------------------------------- | ------------------------------------------------------------ |
| Abstract-expressionism | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=MzNkMDk1OTgwMTUyYThkMmI4Njg1MDUzOTkxYzcwNDlfVlY0RGdkZmRWbVpXNHVXM1BkWEhmYUk5THNwNGpCeldfVG9rZW46TzNJVmJObHp3b0diNGp4YXlVaGNZMW1JbkhjXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=Nzc1YjY2NGFhYmExN2M1YmViZWQ5MTY5MjEwMDcxMTFfcWlSSklCZDlEUEJINjR1WklWUGNBVEoxNWpYNzFVcHdfVG9rZW46SnlLZ2JCcWx3b1VxY3N4UHFISmM3aUZybm9mXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) |
| Baroque                | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=OTNjYjk2ZWM0NjkxZTY4NDNjNzNlMWY5NzRlZmMxODNfTGxpdGFhTkNHOGhqY2RHQjZoUnlmaTVzMm9VUmMzQnpfVG9rZW46RUhUVmJ2OThIbzlZUXZ4aHJHNGNEalVibjFnXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=ZGUwNTU4NjZlZTEyYWQ5Mjc2NjgyOGNjNzc0MWNhZWRfdjNxbkRHWE9ISXAxa2VINUc4amVZaUNIcVVNSHA2UzVfVG9rZW46WXgwTWJPMmcwb0ZuVmR4dkxSQmNMR3pYbjVjXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) |
| Impressionism          | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=NWZhYjA1M2IxMDc0MzBiY2EzMTljZWY2NGZiMjFmOGJfUEtXSnpsWVNOZVRaUHBnMVh4ZTIydzBpcWZNVzlwbWFfVG9rZW46WjRkVmJ1QnYwb3NPc0F4SEhvdmNhMld4bk0wXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=Y2U4Y2VlMjY5YzNhNDJlOTM2YzkyNzhmNTI2OTZhOTVfWWpNVkxKdHFpV3BJMjZCWGxyZGtqSVlIM3dhRURWMnZfVG9rZW46WDQzRGJEcjhab3A3aVp4VjJCTGMwZ1dlbkNmXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) |
| Realism                | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=MTM2NDE0NjJiM2E4YWFkNjMzZThhOGFmYTRlYmQ2ODZfcUhHQ2R3Yzg0YVRRTlZndVdzSzRRTlRpaTdOeXNJWDlfVG9rZW46R3ZpWWJTcmtEb1BxV1l4aTBjNWNlUVhvbnZjXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=OTNmNWE4NmY2OTFhZTE0ZjhiNmY4Mzg1ODNkZjJlY2NfSU1JejhGbkRGYW5xa1NsSE9ka0R4dEc4QVNsc3JhOEpfVG9rZW46VUtrQ2JKWFRtb1ROUFN4YlY0SGNVQkJmblZmXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) |
| Romanticism            | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=NzIzNWYxNmI4YjMxYzQ0NjIxMGJjNjMzNzM1MjliNDJfUVk3NHZaZHFSOHZaMFdQS3N0cFp3QWJLeGdHUjBYQWZfVG9rZW46T25UNGJGTFVub1dma2x4YjBObmNsN1VQbkhjXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=NTRiNzU5MDAxMjE5NmZkMGM3NTc0NjJjZjdkMWNlZTVfd3pDMUt1WWI4dEloU05tVGJPWHpZcWJ4VFY5RFBnVG1fVG9rZW46UmxMQmJBRlBIb0ZnUFd4bGdVNmM4Tm9CbjFkXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) |
| Surrealism             | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=YmE3MjlkYzEyNjgxZTQ5MGU1NWQ0OTZjYWI1MWZmNGVfaWVlZzI2cDZyQldNaElnMjBlTU9OcUtiNWUzS29RSkdfVG9rZW46WGVUcmI2eFRvb1JyU3R4bTRVMWNKMU1abk1kXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) | ![img](https://rcnc6338zx5i.feishu.cn/space/api/box/stream/download/asynccode/?code=NzEwNWZiMWVmZWNmY2Q5YzQ0MTZmNjliZmI3YTAyZmRfZnNYODdyQ3RtZmxORVpsY2JMaThraTJPYjZuZUlYYkxfVG9rZW46UG11NGJXdUMwb2twVFd4QUVFOGNmczIzbkZrXzE3NTI0NzQ2NDY6MTc1MjQ3ODI0Nl9WNA) |
| total                  |                                                              |                                                              |



## 📈 Citation

If you use this dataset in your research, please cite our paper:

```
bibtex
/
```



## 🔍 Related Work

- [Painting-91 Dataset]
  - Khan, Fahad Shahbaz, et al. "Painting-91: a large scale database for computational painting categorization." *Machine vision and applications* 25.6 (2014): 1385-1397.
- [Pandora Style Dataset]
  - Florea, Corneliu, et al. "Pandora: Description of a painting database for art movement recognition with baselines and perspectives." *2016 24th European Signal Processing Conference (EUSIPCO)*. IEEE, 2016.
- [WikiArt Dataset]
  - Saleh, Babak, and Ahmed Elgammal. "Large-scale classification of fine-art paintings: Learning the right metric on the right feature." *arXiv preprint arXiv:1505.00855* (2015).



## 📬 Contact

For questions, feel free to contact:
 📧 202421055240@mail.scut.edu.cn
