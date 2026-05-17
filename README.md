# Random Forest — Chapter 7 (Iris Dataset)

Demo thực hành **Random Forest** với bộ dữ liệu Iris: phân loại loài hoa (classification) và dự đoán độ dài cánh hoa (regression).

## Nội dung repository

| File | Mô tả |
|------|--------|
| `Chapter7_demo_classification_iris.ipynb` | `RandomForestClassifier` — dự đoán loài Iris từ 4 đặc trưng |
| `Chapter7_demo_regression_iris.ipynb` | `RandomForestRegressor` — dự đoán `petallength` từ `petalwidth` |
| `Iris.xls` | Dữ liệu Iris (150 mẫu) |
| `requirements.txt` | Thư viện Python cần cài |

## Kết quả mô hình (tham khảo)

### Classification
- **Accuracy (4 đặc trưng):** ~95.6%
- **Accuracy (2 đặc trưng: petallength, petalwidth):** ~88.9%
- Đặc trưng quan trọng nhất: `petallength`, `petalwidth`

### Regression
- **R² train:** ~0.964 | **R² test:** ~0.940
- **MSE test:** ~0.197
- Ví dụ: `petalwidth = 0.25` → `petallength ≈ 1.44`

## Cài đặt

```bash
git clone https://github.com/nguyenhuuniem12022005/random-forest.git
cd random-forest
pip install -r requirements.txt
```

**Yêu cầu:** Python 3.10+

## Chạy notebook

1. Mở thư mục project trong VS Code / Cursor / Jupyter.
2. Chọn kernel Python đã cài đủ thư viện.
3. Chạy **Run All** trên từng notebook.

> Các notebook đã được chạy sẵn và lưu output. Nếu chạy lại trên máy local, bỏ comment ô Google Colab (nếu có) — không cần thiết khi chạy local.

## Cấu trúc dữ liệu `Iris.xls`

| Cột | Ý nghĩa |
|-----|---------|
| `sepallength` | Chiều dài đài hoa |
| `sepalwidth` | Chiều rộng đài hoa |
| `petallength` | Chiều dài cánh hoa |
| `petalwidth` | Chiều rộng cánh hoa |
| `iris` | Nhãn loài: Iris-setosa, Iris-versicolor, Iris-virginica |

## Thư viện chính

- [scikit-learn](https://scikit-learn.org/) — `RandomForestClassifier`, `RandomForestRegressor`
- pandas — đọc Excel, xử lý dữ liệu
- matplotlib — biểu đồ feature importance / scatter plot

## Tác giả

**Nguyễn Hữu Niêm** — [GitHub](https://github.com/nguyenhuuniem12022005)

## License

Dùng cho mục đích học tập (LDS6 Machine Learning).
