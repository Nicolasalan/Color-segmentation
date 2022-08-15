# Color Segmentation

Esse repositório é um pacote no ROS 1 que implementa um segmentador de cores. Esse pacote possui uma interface com ROS para visualização da segmentação e um serviço para que somente mostra o centroide da segmentação.

**Requisitos**

Antes de executar o pacote, primeiro tem que calibrar a segmentação para o seu caso de uso, para isso utilizo o https://github.com/abhisavaliya/hsv_calibration/.

```
pip install hsv-calibration 
```
Assim que calibrar o pacote,  executar os comandos.
```
git clone https://github.com/Nicolasalan/Color-segmentation.git
cd Color-segmentation
pip3 install -r requirements.txt
```
Depois de instalar o pacote, compilar com o comando abaixo.
```
cd src
source devel/setup.bash
catkin_make
```
**Para iniciar o node e o servico.**
```
Inicia o serviço de segmentação:
rosrun Color-segmentation blob_detection
```
Inicia o node de visualização:
```
rosrun Color-segmentation blob_visualize
```

