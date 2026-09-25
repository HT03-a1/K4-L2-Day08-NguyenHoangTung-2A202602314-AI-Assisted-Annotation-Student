# Bảng so sánh các vòng

Tập kiểm thử: 20 ảnh, 403 box tham chiếu (bỏ qua 14 box cao dưới 16 px). Ngưỡng IoU 0.5; P, R, F1 tính tại conf 0.25.

| Chỉ tiêu             | Vòng 0                                  | Vòng 1                                           |
| :------------------- | :-------------------------------------- | :----------------------------------------------- |
| model                | yolov8n cold start (COCO car+bus+truck) | yolov8n fresh fine-tune, revised CVAT, 50 epochs |
| ảnh train            | 0                                       | 12                                               |
| box train            | 0                                       | 321                                              |
| AP50                 | 0.771                                   | 0.511                                            |
| Δ AP50 so cold start | —                                       | -0.261                                           |
| P@0.25               | 0.925                                   | 1.000                                            |
| R@0.25               | 0.489                                   | 0.199                                            |
| F1                   | 0.640                                   | 0.331                                            |
| R small              | 0.182                                   | 0.000                                            |
| R medium             | 0.547                                   | 0.213                                            |
| R large              | 0.561                                   | 0.415                                            |
