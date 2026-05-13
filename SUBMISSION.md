# Hướng Dẫn Nộp Bài - GPU FinOps Lab

## Tổng quan

Sinh viên cần hoàn thành toàn bộ các phần trong notebook `gpu_finops_lab.ipynb` và nộp các báo cáo cùng hình ảnh minh họa theo yêu cầu dưới đây.

## ⚠️ Bước quan trọng: Nhập thông tin sinh viên

**TRƯỚC KHI BẮT ĐẦU**, sinh viên cần thực hiện các bước sau:

1. Mở notebook `gpu_finops_lab.ipynb`
2. Tìm **Cell 2.5: Student Information Setup** (sau Cell 2)
3. Điền thông tin của bạn vào 2 biến:
   ```python
   STUDENT_NAME = "Nguyen Van A"  # <-- Điền tên của bạn
   STUDENT_ID = "MSSV123456"     # <-- Điền MSSV của bạn
   ```
4. Chạy cell này để hiển thị header với thông tin của bạn
5. **TRONG MỌI SCREENSHOT**, đảm bảo header này hiển thị ở đầu màn hình

**Lưu ý:** Header sẽ có màu gradient (từ xanh đến tím) với tên và MSSV của bạn. Đây là bằng chứng xác định bài làm của bạn.

## Các phần cần hoàn thành

### Part 1: GPU Cluster Monitoring
- **Yêu cầu**: Chạy Cell 3 và Cell 4 để quan sát trạng thái cluster
- **Báo cáo cần nộp**:
  - Screenshot kết quả Cell 3 (View Cluster Nodes) - hiển thị thông tin các GPU nodes
  - Screenshot kết quả Cell 4 (Cluster Metrics Summary) - hiển thị metrics tổng hợp
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

### Part 2: Workload Submission & Cost Tracking
- **Yêu cầu**: Chạy Cell 5 và Cell 6 để submit workloads và record billing
- **Báo cáo cần nộp**:
  - Screenshot kết quả Cell 5 (Submit multiple workloads) - hiển thị trạng thái các workloads
  - Screenshot kết quả Cell 6 (Record billing for workloads) - hiển thị billing summary
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

### Part 3: Spot Instance Management
- **Yêu cầu**: Chạy Cell 7, Cell 8, và Cell 9 để quản lý spot instances
- **Báo cáo cần nộp**:
  - Screenshot kết quả Cell 7 (Check spot pricing) - bảng giá spot hiện tại
  - Screenshot kết quả Cell 8 (Request spot instances) - kết quả request spot instances
  - Screenshot kết quả Cell 9 (Simulate spot preemption) - báo cáo savings sau preemption
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

### Part 4: Autoscaling (KEDA-like)
- **Yêu cầu**: Chạy Cell 10 và Cell 11 để cấu hình và trigger autoscaling
- **Báo cáo cần nộp**:
  - Screenshot kết quả Cell 10 (View and update autoscaling policy) - policy trước và sau khi update
  - Screenshot kết quả Cell 11 (Trigger autoscaler evaluation) - 5 cycles evaluation với các action
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

### Part 5: Cost Analysis & Optimization
- **Yêu cầu**: Chạy Cell 12, Cell 13, Cell 14, và Cell 15 để phân tích cost
- **Báo cáo cần nộp**:
  - Screenshot kết quả Cell 12 (Take cost snapshots) - 5 snapshots với waste percentage
  - Screenshot kết quả Cell 13 (Waste Report) - báo cáo waste analysis
  - Screenshot kết quả Cell 14 (Get Optimization Recommendations) - danh sách recommendations
  - Screenshot kết quả Cell 15 (Full Dashboard View) - dashboard tổng hợp
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

### Part 6: Visualization
- **Yêu cầu**: Chạy Cell 16 và Cell 17 để tạo biểu đồ visualization
- **Báo cáo cần nộp**:
  - **File hình ảnh**: `finops_cost_breakdown.png` - biểu đồ cost breakdown
  - **File hình ảnh**: `finops_timeseries.png` - biểu đồ time-series cost tracking
  - Screenshot kết quả Cell 16 (Cost Breakdown Visualization) - 3 subplots
  - Screenshot kết quả Cell 17 (Time-series cost tracking) - stackplot và waste percentage
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

### Part 7: Complete FinOps Workflow
- **Yêu cầu**: Chạy Cell 18 để thực hiện full optimization workflow
- **Báo cáo cần nộp**:
  - Screenshot kết quả Cell 18 (Full FinOps Optimization Workflow) - toàn bộ 7 steps
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

### Part 8: Real GPU Workload trên Kaggle/Colab
- **Yêu cầu**: Chạy Cell 19 đến Cell 26 để train model thực tế trên GPU
- **Báo cáo cần nộp**:
  - Screenshot kết quả Cell 19 (Install dependencies & detect real GPU) - thông tin GPU được detect
  - Screenshot kết quả Cell 20 (GPU Metrics Collection) - diagnostic test results
  - Screenshot kết quả Cell 22 (Train FP32) - summary FP32 training
  - Screenshot kết quả Cell 23 (Train AMP) - summary AMP training
  - Screenshot kết quả Cell 24 (Compare FP32 vs AMP) - bảng comparison và 3 biểu đồ
  - Screenshot kết quả Cell 25 (Report real GPU costs) - báo cáo cost đã gửi lên gateway
  - **File hình ảnh**: `real_gpu_comparison.png` - biểu đồ comparison FP32 vs AMP
  - **File hình ảnh**: `real_gpu_telemetry.png` - biểu đồ GPU telemetry (nếu có)
  - **File hình ảnh**: `cost_per_epoch.png` - biểu đồ cost per epoch
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

### Part 8.5: Advanced GPU Cost Optimization
- **Yêu cầu**: Chạy Cell 27 đến Cell 31 để thực hiện advanced analysis
- **Báo cáo cần nộp**:
  - Screenshot kết quả Cell 27 (Multi-GPU Cost Analysis) - bảng analysis scaling efficiency
  - Screenshot kết quả Cell 28 (Project Cost Forecasting) - forecast với confidence intervals
  - Screenshot kết quả Cell 29 (Optimization Opportunity Analysis) - prioritized recommendations
  - Screenshot kết quả Cell 30 (Integrated Cost Dashboard) - dashboard 2x3 hoặc 3x2
  - Screenshot kết quả Cell 31 (Challenge Exercise) - chiến lược optimization đã thiết kế
  - **File hình ảnh**: `multi_gpu_scaling.png` - biểu đồ multi-GPU scaling efficiency
  - **File hình ảnh**: `project_forecast.png` - biểu đồ project forecast
  - **File hình ảnh**: `optimization_roadmap.png` - biểu đồ optimization roadmap
  - **File hình ảnh**: `advanced_finops_dashboard.png` - dashboard tổng hợp
- **⚠️ QUAN TRỌNG**: Khi chụp screenshot, scroll lên để header thông tin sinh viên (Cell 2.5) hiển thị ở đầu màn hình

## Cấu trúc bài nộp

Tạo một thư mục nộp bài với cấu trúc sau:

```
[StudentName]_GPU_FinOps_Submission/
├── report.pdf                          # Báo cáo phân tích (nếu có yêu cầu)
├── screenshots/
│   ├── part1_cluster_monitoring.png
│   ├── part1_cluster_metrics.png
│   ├── part2_workload_submission.png
│   ├── part2_billing_summary.png
│   ├── part3_spot_pricing.png
│   ├── part3_spot_request.png
│   ├── part3_spot_preemption.png
│   ├── part4_autoscaler_policy.png
│   ├── part4_autoscaler_evaluation.png
│   ├── part5_cost_snapshots.png
│   ├── part5_waste_report.png
│   ├── part5_recommendations.png
│   ├── part5_dashboard.png
│   ├── part6_cost_breakdown_viz.png
│   ├── part6_timeseries_viz.png
│   ├── part7_full_workflow.png
│   ├── part8_gpu_detection.png
│   ├── part8_gpu_metrics_diagnostic.png
│   ├── part8_fp32_summary.png
│   ├── part8_amp_summary.png
│   ├── part8_fp32_vs_amp_comparison.png
│   ├── part8_real_gpu_cost_report.png
│   ├── part85_multi_gpu_analysis.png
│   ├── part85_project_forecast.png
│   ├── part85_optimization_analysis.png
│   ├── part85_integrated_dashboard.png
│   └── part85_challenge_strategy.png
├── generated_charts/
│   ├── finops_cost_breakdown.png
│   ├── finops_timeseries.png
│   ├── real_gpu_comparison.png
│   ├── real_gpu_telemetry.png          (nếu có)
│   ├── cost_per_epoch.png
│   ├── multi_gpu_scaling.png
│   ├── project_forecast.png
│   ├── optimization_roadmap.png
│   └── advanced_finops_dashboard.png
└── notebook/
    └── gpu_finops_lab.ipynb            # Notebook đã chạy hoàn chỉnh
```

## Nội dung báo cáo (Report)

Nếu có yêu cầu viết report, bao gồm các phần sau:

### 1. Giới thiệu
- Mục tiêu của bài lab
- Tổng quan về GPU FinOps

### 2. Phân tích từng phần
- **Part 1-7**: Phân tích kết quả từ mock cluster
  - Cluster monitoring insights
  - Cost tracking observations
  - Spot instance savings analysis
  - Autoscaling behavior
  - Waste analysis và recommendations
- **Part 8**: Phân tích real GPU training
  - FP32 vs Mixed Precision (AMP) comparison
  - Cost savings achieved
  - GPU utilization patterns
- **Part 8.5**: Advanced analysis
  - Multi-GPU scaling efficiency
  - Project cost forecasting
  - Optimization strategy prioritization

### 3. Kết luận và học hỏi
- Những kỹ năng FinOps đã học
- Các chiến lược cost optimization hiệu quả
- Ứng dụng thực tế trong projects

## Tiêu chí đánh giá

- **Hoàn thành đầy đủ**: Tất cả 8.5 parts đều đã chạy thành công
- **Chất lượng screenshot**: Rõ nét, đầy đủ thông tin
- **Phân tích**: Có giải thích và comment về kết quả (nếu có report)
- **Visualization**: Biểu đồ được tạo và lưu đúng format
- **Code**: Notebook chạy không lỗi, outputs được lưu

## Lưu ý quan trọng

1. **Gateway URL**: Đảm bảo thay đổi `GATEWAY_URL` trong Cell 2 với tunnel URL của bạn
2. **GPU Environment**: Part 8 cần chạy trên Kaggle/Colab với GPU enabled. Nếu không có GPU, có thể skip phần này nhưng cần ghi chú rõ
3. **File naming**: Đặt tên file screenshot theo đúng cấu trúc để dễ đánh giá
4. **Notebook state**: Nộp notebook với tất cả outputs đã được chạy (not cleared)
5. **Hình ảnh**: Đảm bảo tất cả file PNG được tạo và nộp đầy đủ

## Hạn chót nộp

- 23:59 PM Wednesday 05/13/2026

## Cách thức nộp

- Gửi link GitHub repository của bạn lên LMS

---
