#Hệ thống Quản lý Giao nhận và Vận chuyển					
##Hiện trạng: Việc vận chuyển hàng hóa chủ yếu dựa vào giấy tờ, ghi chép thủ công, dễ gây nhầm lẫn hoặc thất lạc.		
					
##Mong muốn thay đổi: Tạo hệ thống giúp theo dõi đơn hàng, phân phối, lịch trình vận chuyển, cập nhật trạng thái theo thời gian thực.		
					
##Gợi ý cơ sở dữ liệu: 
      Đơn hàng (OrderID, CustomerID, Ngày đặt hàng, Tổng tiền, Trạng thái)		
			Phân phối (DeliveryID, OrderID, DriverID, Phương tiện, Ngày vận chuyển, Trạng thái)		
			Tài xế (DriverID, Name, Phone, LicensePlate)		
			Hàng hóa (ProductID, Name, Quantity, Đơn vị)		
			Kho hàng (WarehouseID, Location, Capacity, Trạng thái)		
			Vật tư vận chuyển (TransportMaterialID, Name, Quantity, Usage)		
			Lịch trình giao hàng (ScheduleID, DeliveryID, ExpectedDate, ActualDate)		
			Trạng thái vận chuyển (StatusID, Description)		
			Đánh giá dịch vụ (FeedbackID, CustomerID, Rating, Comments)		
			Lịch sử vận chuyển (HistoryID, DeliveryID, Events, Timestamp)		
##Chức năng:			
      Quản lý đặt hàng, chuyển phát		
			Theo dõi trạng thái vận chuyển theo thời gian thực		
			Quản lý lịch trình, phân phối tài xế và phương tiện		
			Báo cáo thống kê vận chuyển, số lượng hàng, thời gian giao hàng		
			Gửi thông báo cập nhật trạng thái khách hàng		
			Quản lý kho hàng liên quan đến vận chuyển		
			Quản lý phí vận chuyển và thanh toán		
			Đánh giá dịch vụ vận chuyển		
