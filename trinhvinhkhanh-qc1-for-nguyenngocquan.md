# Phiếu QC 1 — Road v1.0

Lô được kiểm (học viên):  Trần Ngọc Quân (2A202603250)   
Người kiểm (học viên):  Trịnh Vinh Khánh (2A202603220)
Ngày: 21/11/2026                         
Phiên bản guideline: Road v1.0  
File được kiểm (tên + `revision` trong manifest):   nguyenngocquan-front.zip, nguyenngocquan-fisheye.zip — revision 2 (sha256 khớp manifest)

Số ảnh kiểm: 6 (A04, A06, A08, A09, A13, B03 + 0 ảnh thêm, ghi riêng)   Số nhãn đã kiểm (shape + tag): 89 (65 shape + 24 tag)

## Tổng hợp theo mã
| Mã | Loại lỗi | Số mục kiểm | Số lỗi | Mức |
| --- | --- | ---: | ---: | --- |
| QC1-01 tag camera | sai thuộc tính / bỏ sót | 6 | 0 | nặng |
| QC1-02 đủ L1, R1 | bỏ sót | 5 | 1 | nặng |
| QC1-03 position | sai thuộc tính / thừa | 15 | 0 | nặng |
| QC1-04 tâm vạch, chiều, điểm dừng | sai phạm vi / bỏ sót | 19 | 0 | chính |
| QC1-05 vạch đứt, che | sai phạm vi / sai thuộc tính | 15 | 0 | chính |
| QC1-06 style, color, kind | sai thuộc tính | 15 | 0 | chính |
| QC1-07 vùng lái | sai phạm vi / bỏ sót / thừa | 13 | 2 | chính |
| QC1-08 đèn, màu | bỏ sót / sai phạm vi / sai thuộc tính | 15 | 0 | nặng / chính |
| QC1-09 facing, type, group, biển phụ | sai thuộc tính | 13 | 0 | chính |
| QC1-10 hình in, đủ biển | bỏ sót / sai phạm vi | 13 | 0 | chính |
| QC1-11 fisheye | sai phạm vi / sai thuộc tính | 3 | 0 | chính |
| QC1-12 file | lỗi file | 2 | 0 | nhẹ / nặng |

## Danh sách lỗi (mỗi lỗi một dòng)
| # | Mã | Ảnh | Nhãn (label, id) | Mức | Mô tả ngắn |
| --- | --- | --- | --- | --- | --- |
| 1  | QC1-07  | A06 | drivable | chính | thiếu khu vực drivable |
| 2  | QC1-07  | A08 | drivable | chính | thiếu khu vực drivable |
| 2  | QC1-02  | A09 | thiếu lane L1 | nặng | làn đôi cần có 2 polyline lane và cả 2 dùng thuộc tính double |


## Ca mơ hồ
| Ảnh | Câu hỏi cho lead | Lời đáp (nếu có) |
| --- | --- | --- |
| A13 | Kính xe có nước mưa, nhưng thời tiết không mưa, thuộc tính của tag weather có được tính là overcast không? | --- |

## Quyết định
Lỗi nặng: 1   Lỗi chính: 2 / 89 nhãn = 2,25 %   Lỗi nhẹ: 0   Ca chờ lead: 1  
Quyết định (Release / Hold / Rework):  Rework
Lý do (theo luật của phiếu): Theo Luật quyết định: Có ít nhất một lỗi nặng → **Rework**.

Loại lỗi: bỏ sót = thiếu nhãn phải có; thừa = gán cái không phải đối tượng; sai phạm vi = hình lệch, sai chiều, dừng sai chỗ, tràn vùng. Ba loại này theo cách chia lỗi gán nhãn của ISO/IEC 5259-4 (mục 8.4.2); "sai thuộc tính" và "lỗi file" là khóa học thêm. Cách xếp mức: [thang mức lỗi](../docs/qc_severity_road_v1.0.md).
