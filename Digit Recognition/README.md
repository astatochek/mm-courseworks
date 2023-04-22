# Распознавание образов с помощью Pytorch
### Библиотеки
Для подключения необходимых библиотек ввести в первую же ячейку следующий код и запустить:

Linux
```cmd
!pip install numpy matplotlib torch==1.7.0+cpu torchvision==0.8.1+cpu torchaudio==0.7.0 -f https://download.pytorch.org/whl/torch_stable.html
```
Windows
```cmd
!pip install numpy matplotlib torch==1.7.0+cpu torchvision==0.8.1+cpu torchaudio==0.7.0 -f https://download.pytorch.org/whl/torch_stable.html
```
MacOS
```cmd
!pip install numpy matplotlib torch torchvision torchaudio
```
### Загрузка обученной нейросети
Для загрузки обученной нейросети, результаты которой описаны в отчете написать в любой ячейке
```python
model = MnistModel(input_size, hidden_size=32, out_size=num_classes)
model.load_state_dict(torch.load('model.pth'))
```
и пропустить шаги тренировки, а сразу перейти к тестированию на отдельных изображениях.