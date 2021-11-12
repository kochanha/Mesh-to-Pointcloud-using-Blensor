# Mesh to Point Cloud GT

main concept : produced by referring to the data generation part of the [Points2surf](https://github.com/ErlerPhilipp/points2surf)  
Generating Point Cloud by using Blensor (ToF Simulator)

### 1. 환경 설정
```
git clone https://github.com/kochanha/Mesh-to-Pointcloud-using-Blensor.git
cd mesh2pc

# create conda env
conda env create --file p2s.yml

# activate the new conda environment
conda activate p2s
```
### 2. Load OBJ Mesh Files
```
cd datasets
```
Make it the same as the example file format and store the obj file in the "00_base_meshes" folder.

### 3. Add Blensor Appimage
```
cd bin

# Download Blensor Appimage
wget https://www.blensor.org/dload/Blensor-x64.AppImage
```

### 4. Modify Code (Will be fully automated later)
Open "make_dataset.py"  
![image](https://user-images.githubusercontent.com/44921488/126310755-037f0b54-e98a-4e65-ab0e-d8fdf96122ba.png)  
datasets = [ "" ] # modification is mandatory

### 5. Run Code
```
python make_dataset.py
```

### 6. Results
![image](https://user-images.githubusercontent.com/44921488/126311278-d34195df-d924-4ad2-b0d4-a90787222ecc.png)
![image](https://user-images.githubusercontent.com/44921488/126311466-c7d84f09-a52e-48d2-9805-330bf0d07488.png)
