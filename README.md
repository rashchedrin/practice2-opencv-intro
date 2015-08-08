# �������������� ��� ���������� �������� �� ������� ���������� ������������� ������ OpenCV

[![Build Status](https://travis-ci.org/Itseez-NNSU-SummerSchool2015/practice2-opencv-intro.svg)](https://travis-ci.org/Itseez-NNSU-SummerSchool2015/practice2-opencv-intro)


������ ������������ ����� �������������� ��� �������� ����� ������ � ����������� OpenCV:
  - ��������/���������� ����������� (������� ��������� � �������� ������ ```opencv_core```).
  - ��������� ����������� � ������� ��������� �������� ���������� (�������� ������ ```opencv_imgproc```).
  - ���������� ����������� ���������� ���������� ���������� (������� �������� ������ ```opencv_highgui```).

## ����� ��������� �������

��������� �������:
  - ```3rdparty``` - ���������� gtest.
  - ```include``` - ���������� ��� ���������� ������������ ������.
  - ```samples``` - ���������� ��� ���������� �������� �������������.
  - ```src``` - ���������� � ��������� ������.
  - ```test``` - ���������� � �������.
  - ```.gitignore``` - �������� ���������� ������, ������� �� ������������� � ������.
  - ```.travis.yml``` - ���������������� ���� ��� ������� ��������������� ������������ Travis-CI.
  - ```CMakeLists.txt``` - ����� ���� ��� ������ ������� � ������� CMake.
  - ```README.md``` - ���������� � �������, ������� �� ������ �������.

� ��������� ������� ������� ��������� ������:
  - ������ ��������������� ������� (```./include/auxiliaries.hpp```, ```./src/auxiliaries.hpp```), � ���������, ������� ��������� ���������� ��������� ������.
  - ������, ���������� ���������� � ���������� ������� ��������, ��������� � ����������� ����������� (```./include/img_proc.hpp```, ```./src/img_proc.hpp```).
  - ������� ������ (```aux_test.cpp```).
  - ������ ����������, ��������� ��������� ������ (```sample_template.cpp```).

## ���� � ������

**_���� ������ ������_** - ������� ������� ��������� ������ ```opencv_core``` � ���������� �������� ��������� ����������� ������ ```opencv_imgproc```, ��������� ������������� ��������� ���������� ������ ```opencv_highgui``` �� ������� ������ ����������� ����� �� �����������.

��� ����� ���������� ������ ��������� **_������_**:
  1. ������� ������� ������ ������ ```Mat``` (������ ```opencv_core```), ������� ����������� ��� ������������� �����������.
  2. ����������� �������� �������� ������ � �������������:
     1. �������� ����������� (� ������� ������������� ��� ������ ```create``` ������ ```Mat```).
	 2. �������� ����������� (������� ```imread```).
	 3. ���������� ����������� (������� ```imwrite```).
	 4. ����������� ����������� (������� ```imshow```, ```waitKey```).
	 5. ����������� ����������� (����� ```copyTo``` ������ ```Mat```).
	 6. ������ ���������� (��������, ����������� � ��.).
	 7. �������������� ����������� � ��������� �������� ������������ (������� ```cvtColor```).
  3. ������� � ����������� � �������������� OpenCV ��������� ������� ��������� �������� �� �����������:
     1. ����������� ����������� (������� ```threshold```) + ����� �������� (������� ```findContours```). ����������: ��� ����������� �������� ������� ������������ ������� ```drawContours```.
	 2. ��������������� �������� (������� ```morphologyEx```).
	 3. �������� ������ (������� ```Sobel```).
	 4. �������� ������� (������� ```Laplacian```).
	 5. �������� ����� ����� (������� ```Canny```). ����������: ����� ����������� ������� ����� ����������� ��������� ���������� � �������������� ���������� � ������� ������.
  4. ����������� ����������� ���������, ��������������� ��������� �����������:
     1. ����������� ��������� �����������.
	 2. ����������� �����������, �� ������� ���������� �������.
	 3. ������� ������ �������������� (������) ��� ���������� ��������� ������� ��������� ��������.

## ���������� �� ���������� ������

  1. ������� ������� �� [github.com](https://github.com), ���� ����� �����������. ��� �������������� ��������� ������� ```github-account```.
  
  2. ������� fork ����������� ```https://github.com/Itseez-NNSU-SummerSchool2015/practice2-opencv-intro``` (� ������������ Git upstream-�����������) � ���� � ����������� � ��������� github-account. � ���������� ����� ������� ����� ����������� � ��������� ```https://github.com/github-account/practice2-opencv-intro``` (origin-�����������).
  
  3. ����������� ����������� ```https://github.com/github-account/practice2-opencv-intro```, ���������������� ��������� ��������:
  
  ```
  $ git clone https://github.com/github-account/practice2-opencv-intro
  ```
  
  4. ��������� upstream-�����������:
  
  ```
  $ git remote add upstream https://github.com/github-account/practice2-opencv-intro
  ```
  
  5. ��������� ��� ������������, �� ��� �������� ����� ����������� ��� �������� � ������������ Git:
  
  ```
  $ git config --global user.name "github-account"
  ```
  
  6. ������� ����� find-contours-implementation � ������� � ���:
  
  ```
  $ git checkout -b find-contours-implementation
  ```
  
  7. � ����� ```find-contours-implementation``` ��������� ���������� ��������� ������� ������ ��������, ������� ���� ������������� ��� ����������� ������� ������.

  8. ������� ����� gui-implementation � ������� � ���:
  
  ```
  $ git checkout -b gui-implementation
  ```
  
  9. � ����� ```gui-implementation``` ��������� ������������� ������������ �����. ����������: �� �������� ���������� ����������� ������ ������������� ���������� ������ ��������.
  
  10. ����� ��������� ������ ���������� ������ �� ��������� ��������� ����������������� ������ � ����������� ��������� � �����.
  
  ```
  $ git commit [-m "<message_to_commit>"] [-a]
  [-a] - ������������� ��������� ��������� ��� ������������ �� ������� ������ ��� ���������� ������� git add
  [--amend] - �������������� ��������� ������ (������������, ���� �� ������ ���������)
  ```
  
  ```
  git push origin <branch-name>
  ```
  
  11. �� �������� ������� Pull Request, ����� ��������� ����������������� ������ �� Travis-CI � ��������� �������������� ������� ����� ������ ����.
  
  ����������: ��������� ���������� �� ������ �������, ������� ������ ���� ������� � [������������ ������ �� �������� ������������ ����������](https://github.com/Itseez-NNSU-SummerSchool2015/practice1-devtools).