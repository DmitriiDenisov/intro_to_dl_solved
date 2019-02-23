# Introduction to Deep Learning course resources
https://www.coursera.org/learn/intro-to-deep-learning

Здесь все решения для недель 1-5

Здесь нет папки Readonly. Она и не нужна, это старая версия курса. Если вдруг она понадобится, то можно взять на курсере, либо вызовом функция из ```link_all_keras_resources.py```

Если не работает строка
```download_utils.link_all_keras_resources()```
то просто удалить её. Вообще она не нужна, её можно удалить везде

## Running on Google Colab (tested for all weeks)
Google has released its own flavour of Jupyter called Colab, which has free GPUs!

Here's how you can use it:
1. Open https://colab.research.google.com, click **Sign in** in the upper right corner, use your Google credentials to sign in.
2. Click **GITHUB** tab, paste https://github.com/hse-aml/intro-to-dl and press Enter
3. Choose the notebook you want to open, e.g. week2/v2/mnist_with_keras.ipynb
4. Click **File -> Save a copy in Drive...** to save your progress in Google Drive
5. Click **Runtime -> Change runtime type** and select **GPU** in Hardware accelerator box
6. **Execute** the following code in the first cell that downloads dependencies (change for your week number):
```python
! shred -u setup_google_colab.py
! wget https://raw.githubusercontent.com/hse-aml/intro-to-dl/master/setup_google_colab.py -O setup_google_colab.py
import setup_google_colab
# please, uncomment the week you're working on
# setup_google_colab.setup_week1()
# setup_google_colab.setup_week2()
# setup_google_colab.setup_week3()
# setup_google_colab.setup_week4()
# setup_google_colab.setup_week5()
# setup_google_colab.setup_week6()

# If you're using the old version of the course (check a path of notebook on Coursera, you'll see v1 or v2),
# use setup_week2_old().
```
