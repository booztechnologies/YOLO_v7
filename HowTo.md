# How To

## Steps to run Code

- Clone the repository.

```shell
git clone git@github.com:booztechnologies/YOLO_v7.git
```

- Go to cloned folder.

```shell
cd YOLO_v7
```

- Create a virtual envirnoment (Recommended, If you dont want to disturb python packages)

```shell
### For Linux Users

python3 -m venv .env
source .env/bin/activate

### For Window Users

python3 -m venv .env
.env\Scripts\activate
```

- Upgrade pip with mentioned command below.

```shell
### For Linux Users

pip install --upgrade pip

### For Window Users
pyhton -m pip install --upgrade pip
```

- Install requirements with mentioned command below.

```shell
pip install -r requirements.txt
pip install scikit-image
pip install filterpy
```

- Download [yolov7](https://hellobooz.sharepoint.com/:f:/s/EmbeddedSystems/EkTh1FMytAxCnjq_J8u3KkMBlgcB7iZA80FVqwzdZRnzjQ?e=QYgtZu) object detection weights from link and move them to the working directory

- Run the code with mentioned command below.

```shell
#if you want to change source file
python detect_and_track.py --weights yolov7.pt --source .\inference\images\horses.jpg
python detect_and_track.py --weights yolov7.pt --source .\inference\images\people_group.jpg

#for specific class (person)
python detect_and_track.py --weights yolov7.pt --source .\inference\videos\people.mp4 --classes 0
```
