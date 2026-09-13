# Support Vector Machine - Iris Classification

## 1. Giới thiệu

Đây là project môn Học máy cơ bản, sử dụng thuật toán **Support Vector Machine (SVM)** để phân loại hoa Iris.

Project được thực hiện trên **Google Colab** với thư viện **Scikit-learn**.

## 2. Dataset

Sử dụng bộ dữ liệu **Iris Dataset** được cung cấp bởi Scikit-learn.

Dataset gồm 3 loại hoa:

- Setosa
- Versicolor
- Virginica

Mỗi mẫu hoa có 4 đặc trưng:

- Sepal Length
- Sepal Width
- Petal Length
- Petal Width

Dữ liệu được chia thành:

- 120 mẫu cho tập huấn luyện
- 30 mẫu cho tập kiểm tra

## 3. Phương pháp

Quy trình thực hiện:

1. Load Iris Dataset
2. Khám phá và trực quan hóa dữ liệu
3. Chia dữ liệu thành tập train/test
4. Chuẩn hóa dữ liệu bằng StandardScaler
5. Huấn luyện mô hình SVM
6. Dự đoán trên tập kiểm tra
7. Đánh giá mô hình bằng Accuracy và Classification Report
8. Trực quan hóa Confusion Matrix
9. Thử dự đoán một mẫu hoa mới

### Cấu hình mô hình SVM

- Kernel: RBF
- C: 1.0
- Gamma: scale

## 4. Kết quả

Mô hình đạt độ chính xác:

**96.67%**

Confusion Matrix:

| Actual / Predicted | Setosa | Versicolor | Virginica |
|---|---:|---:|---:|
| Setosa | 10 | 0 | 0 |
| Versicolor | 0 | 9 | 1 |
| Virginica | 0 | 0 | 10 |

Mô hình chỉ phân loại nhầm **1 mẫu Versicolor thành Virginica** trên 30 mẫu kiểm tra.

## 5. Dự đoán mẫu mới

Với mẫu:

[5.1, 3.5, 1.4, 0.2]

Mô hình dự đoán:

**Setosa**

## 6. Công nghệ sử dụng

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- Seaborn
- Scikit-learn
- Support Vector Machine

## 7. Cách chạy

Mở file SVM_Iris.ipynb bằng Google Colab và chạy các cell theo thứ tự từ trên xuống dưới.

## 8. File trong project

`	ext
SVM-Machine-Learning/
├── README.md
├── requirements.txt
├── .gitignore
└── SVM_Iris.ipynb
9. Tác giả

Project được thực hiện cho môn Học máy cơ bản.
