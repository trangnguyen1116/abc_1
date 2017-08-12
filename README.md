<script type="text/javascript" src="https://www.gstatic.com/charts/loader.js"></script>

<script type="text/javascript">
  google.charts.load("current", {packages:["timeline"]});
  google.charts.setOnLoadCallback(drawChart);
  function drawChart() {

    var container = document.getElementById('example3.1');
    var chart = new google.visualization.Timeline(container);
    var dataTable = new google.visualization.DataTable();
    dataTable.addColumn({ type: 'string', id: 'Position' });
    dataTable.addColumn({ type: 'string', id: 'Name' });
    dataTable.addColumn({ type: 'date', id: 'Start' });
    dataTable.addColumn({ type: 'date', id: 'End' });
    dataTable.addRows([
 ['Vận hành nhà vắt 80 điểm', 'Hoàn thành xây dựng và lắp đặt nhà vắt 80 điểm',  new Date(2017, 7, 1), new Date(2017, 9, 31)],
['Vận hành nhà vắt 80 điểm', 'Đào tạo và vận hành nhà vắt 80 điểm',  new Date(2017, 9, 31), new Date(2017, 10, 15)],
['Vận hành nhà vắt 10 điểm', 'Hoàn thành xây dựng và lắp đặt nhà vắt 10 điểm',  new Date(2017, 5, 15), new Date(2017, 7, 25)],
['Vận hành nhà vắt 10 điểm', 'Đào tạo và vận hành nhà vắt 10 điểm',  new Date(2017, 7, 25), new Date(2017, 8, 9)],
['Tư vấn kỹ thuật chăn nuôi', 'Lựa chọn tư vấn phù hợp',  new Date(2017, 7, 1), new Date(2017, 8, 15)],
['Tư vấn kỹ thuật chăn nuôi', 'Nhận kiến thức từ tư vấn',  new Date(2017, 8, 15), new Date(2018, 0, 13)],
['Tư vấn kỹ thuật chăn nuôi', 'Cải tiến chăn nuôi và nhân đàn sử dụng kiến thức tư vấn',  new Date(2017, 8, 15), new Date(2018, 0, 13)],
['Chuẩn hóa thu mua và cung ứng', 'Tìm hiểu hiện trạng cung ứng (chậm trong cung cấp)',  new Date(2017, 7, 13), new Date(2017, 7, 23)],
['Chuẩn hóa thu mua và cung ứng', 'Lên quy trình thu mua và cung ứng - Test 1',  new Date(2017, 7, 23), new Date(2017, 7, 26)],
['Chuẩn hóa thu mua và cung ứng', 'Lấy ý kiến quy trình thử',  new Date(2017, 7, 26), new Date(2017, 7, 30)],
['Chuẩn hóa thu mua và cung ứng', 'Lên quy trình chính thức',  new Date(2017, 7, 30), new Date(2017, 7, 31)],
['Hiện đại hóa quy trình trang trại và báo cáo - Giai đoạn 1', 'AppSheet cho trại',  new Date(2017, 7, 7), new Date(2017, 7, 28)],
['Hiện đại hóa quy trình trang trại và báo cáo - Giai đoạn 1', 'Báo cáo cho các phòng ban liên quan phục vụ công việc quản lý',  new Date(2017, 7, 14), new Date(2017, 7, 28)],
['Hiện đại hóa quy trình trang trại và báo cáo - Giai đoạn 1', 'Đưa quy trình kế hoạch & báo cáo cho cả công ty đi vào hoạt động',  new Date(2017, 7, 28), new Date(2017, 9, 31)],
['Phân tích các mô hình kinh doanh và kế hoạch kinh doanh (dài hạn)', 'Phân tích các mô hình kinh doanh và kế hoạch kinh doanh (dài hạn) - Giai đoạn 1',  new Date(2017, 8, 1), new Date(2017, 9, 1)],
['Phân tích các mô hình kinh doanh và kế hoạch kinh doanh (dài hạn)', 'Phân tích các mô hình kinh doanh và kế hoạch kinh doanh (dài hạn) - Giai đoạn 2',  new Date(2017, 9, 1), new Date(2017, 10, 30)],
['Phân tích các mô hình kinh doanh và kế hoạch kinh doanh (dài hạn)', 'Phân tích các mô hình kinh doanh và kế hoạch kinh doanh (dài hạn) - Giai đoạn 3',  new Date(2017, 10, 30), new Date(2018, 1, 28)],
['Lên quy trình sản xuất và bán hàng', 'Quy trình tạm cho lần bán sữa chưa chính thức ra thị trường',  new Date(2017, 9, 15), new Date(2017, 9, 30)],
['Lên quy trình sản xuất và bán hàng', 'Quy trình chính thức cho nhà máy',  new Date(2017, 9, 30), new Date(2018, 3, 28)],
['Bán sữa chưa chính thức (thanh trùng, tiệt trùng)', 'Tìm nhà máy gia công',  new Date(2017, 7, 14), new Date(2017, 7, 28)],
['Bán sữa chưa chính thức (thanh trùng, tiệt trùng)', 'Tìm công thức (nhiều giai đoạn)',  new Date(2017, 7, 14), new Date(2017, 11, 12)],
['Bán sữa chưa chính thức (thanh trùng, tiệt trùng)', 'Kế hoạch & báo cáo bán hàng (cả kế hoạch thử phản ứng thị trường với các công thức khác nhau)',  new Date(2017, 8, 4), new Date(2017, 9, 4)],
['Bán sữa chưa chính thức (thanh trùng, tiệt trùng)', 'Tìm nhân sự và lập hệ thống phân phối hàng',  new Date(2017, 9, 4), new Date(2018, 0, 2)],
['Bán sữa chưa chính thức (thanh trùng, tiệt trùng)', 'Phân tích các phương án gia công',  new Date(2017, 7, 28), new Date(2017, 8, 4)],
['Bán sữa chua chưa chính thức', 'Tìm nhà máy gia công',  new Date(2017, 7, 14), new Date(2017, 7, 28)],
['Bán sữa chua chưa chính thức', 'Tìm công thức',  new Date(2017, 8, 30), new Date(2017, 11, 29)],
['Bán sữa chua chưa chính thức', 'Phân tích các phương án gia công',  new Date(2017, 7, 28), new Date(2017, 8, 4)],
['Bán sữa chua chưa chính thức', 'Kế hoạch & báo cáo bán hàng (cả kế hoạch thử phản ứng thị trường với các công thức khác nhau)',  new Date(2017, 8, 4), new Date(2017, 9, 4)],
['Bán sữa chua chưa chính thức', 'Tìm nhân sự và lập hệ thống phân phối hàng',  new Date(2017, 9, 4), new Date(2018, 0, 2)],
['Hoàn thành hồ sơ nhà máy', 'Hoàn thành hồ sơ nhà máy',  new Date(2017, 7, 14), new Date(2017, 9, 13)],
['Hoàn thành máy móc thiết bị nhà máy', 'Phân tích tính khả thi máy rót với sản phẩm (kỹ thuật)',  new Date(2017, 7, 14), new Date(2017, 8, 13)],
['Hoàn thành máy móc thiết bị nhà máy', 'Lựa chọn máy rót chai và nguyên liệu chai',  new Date(2017, 8, 13), new Date(2017, 9, 28)],
['Hoàn thành máy móc thiết bị nhà máy', 'Công thức sản phẩm cho quy trình sản xuất',  new Date(2017, 11, 29), new Date(2018, 0, 28)],
['Hoàn thành máy móc thiết bị nhà máy', 'TÌm công nghệ phù hợp',  new Date(2018, 0, 28), new Date(2018, 2, 29)],
['Xây dựng nhà máy', 'Thiết kế',  new Date(2017, 10, 1), new Date(2017, 11, 1)],
['Xây dựng nhà máy', 'Hoàn thành xây dựng nhà máy',  new Date(2017, 11, 1), new Date(2018, 11, 1)],
['Marketing và concept sản phẩm', 'Marketing và concept sản phẩm',  new Date(2017, 7, 14), new Date(2018, 4, 31)],
['Quy trình cho các phòng ban - KT-KS', 'Quy trình kế toán và cải thiện năng lực kế toán công ty',  new Date(2017, 7, 14), new Date(2017, 8, 28)],
['Quy trình cho các phòng ban - KT-KS', 'Quy trình và lập team kiểm soát - giai đoạn chưa bán hàng. Từ giai đoạn bắt đầu bán hàng, qiy trình kiểm soát sẽ được lên sau.',  new Date(2017, 8, 28), new Date(2017, 10, 12)],
['ERP', 'Lựa chọn nhà thầu',  new Date(2017, 7, 14), new Date(2017, 8, 28)],
['ERP', 'Triển khai (kết hợp với nhà thầu, team, và tư vấn nếu có)',  new Date(2017, 8, 28), new Date(2018, 3, 16)],
['Công thức phomat và các sản phẩm khác (sữa chua uống)', 'Công thức phomat và các sản phẩm khác (sữa chua uống)',  new Date(2018, 0, 1), new Date(2018, 2, 2)],
['Phát triển thu mua trong dân', 'Lên kế hoạch cụ thể',  new Date(2018, 7, 21), new Date(2018, 8, 4)],
['Hoạt động trang trại - Măng Đen', 'Kế hoạch (cả dự án và hoạt động thường ngày) trong 1 năm tới',  new Date(2018, 7, 14), new Date(2018, 7, 28)],
['Hoạt động trang trại - Trại 2 & các trại khác', 'Làm sau 15 . 09',  new Date(2018, 8, 15), new Date(2018, 8, 29)]]);
  var options = {
      timeline: { colorByRowLabel: true }
    };
    chart.draw(dataTable);
  }
</script>

<div id="example3.1" style="height: 1000px;"></div>
