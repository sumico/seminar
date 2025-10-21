page 1

dataset: https://wellsr.com/python/fine-tuning-hugging-face-multimodal-transformers-in-pytorch/

<img width="1398" height="749" alt="image" src="https://github.com/user-attachments/assets/aca1b217-136e-4e8d-826f-b89f91d25f67" />

Source: https://wellsr.com/python/fine-tuning-hugging-face-multimodal-transformers-in-pytorch/

---
page 2

Multimodal AI is used for prediction and classification when utilizing different types of data, such as numerical data and text data.

---
page 3

Error message:

Can't load the model for 'facebook/flava-full'. If you were trying to load it from 'https://huggingface.co/models', make sure you don't have a local directory with the same name. Otherwise, make sure 'facebook/flava-full' is the correct path to a directory containing a file named pytorch_model.bin, tf_model.h5, model.ckpt or flax_model.msgpack.

JPN: facebook/flava-full は Hugging Face Hub から削除されており、現在は利用不可。そのため、エラーは「モデルが存在しない」ことが原因。

ENG: facebook/flava-full has been removed from Hugging Face Hub and is currently unavailable. Therefore, the error is caused by the model not existing.

修正方法/How to fix it: 

facebook/flava-full の代わりに、同じ FLAVA 系列のモデルを使う。/Instead of facebook/flava-full, use a model from the same FLAVA family.

from transformers import AutoProcessor, FlavaModel　→　from transformers import FlavaProcessor, FlavaModel

# 旧/old: "facebook/flava-full"

# 新/new: "facebook/flava"

processor = FlavaProcessor.from_pretrained("facebook/flava")

model = FlavaModel.from_pretrained("facebook/flava")

---




