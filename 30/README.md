page 1

MNIST: Image dataset of handwritten numbers

70,000 handwritten numbers “image + label” data 

60,000 for training data (image and label) + 10,000 for test data (image and label)

<img width="777" height="682" alt="image" src="https://github.com/user-attachments/assets/4ae297e5-6e7d-4091-91e7-159f4552d703" />

---

page 2

The image size is 28 x 28 (pixels), and each image data has a correct answer label indicating “which number is written”.

<img width="947" height="708" alt="image" src="https://github.com/user-attachments/assets/567b3269-c109-4f55-8244-6722a683496b" />

---

page 3

Row 1: Correct answer label/Pixel 0 to pixel 783 (=784) pixel value (28 * 28 = 784) (2^8 = 2 to the power of 8 = 256)

The correct answer label contains the correct answer as it is, but convert it to one-hot-encoding 

Example: “3” -> [0, 0, 0, 0, 1, 0, 0, 0, 0, 0, 0]

<img width="972" height="626" alt="image" src="https://github.com/user-attachments/assets/a1070292-b40a-491e-89ad-7ec57591b9a3" />

---
