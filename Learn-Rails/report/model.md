# ***Active Record***
## ***Active Record Basics***
### 1.Create
##### ***creat()*** : tạo mới một collectionerrors.details
##### ***new***
### 2.Read
##### ***all*** : return all collection 
##### ***firts*** :return first collection
##### ***find_by()*** : return collection()
####### ex: return the first user named David
####### david = User.find_by(name: 'David')
##### ***where()*** : return thoả where()
### 3.Update
##### save
##### update()
##### update_all
### 4.Delete
##### destroy 
##### destroy_by() : delete all collection ()
##### destroy_all 
## ***Active Record Validations***
### 1.Create & Save & Update 
##### create & create!
##### save & save!
##### update & update! : Thay đổi cho nhiều trường 
### 2.Skipping 
##### decrement! : Giảm		// decrement_counter 
##### increment! : Tăng   // increment_counter 
##### update_all
##### update_attribute
##### update_column
##### update_columns
##### update_counters
### 3.vaild? & invalid 
### 4.errors[]
### 5.errors.details[:]
### 6.Validate Helpers
##### acceptance: / accerptance{message: } : chấp thuận
##### confirmation: xác nhận
##### inclusion:{} :bao gồm ( chỉ nhận dữ liệu có thoả)
##### length:{ minimum: } // length:{ maximum: } // length:{ in: } //length:{ is: }
##### numericality: true/only_integer
###### ***only_integer***
####### :greater_than 
####### :greater_than_or_equal_to
####### :equal_to
####### :less_than 
####### :less_than_or_equal_to 
####### :other_than 
####### :odd
####### :even 
##### presence : kiểm tra tồn tại // absence : kiếm tra không tồn tại
##### uniqueness: {scope:} (phạm vi) {case_sensitive: } (kiểm tra hoa thường)
##### validates_with: xác thực // validates_each: 
## ***Active Record Callbacks***
### 1 Creating an Object
##### before_validation
##### after_validation
##### before_save
##### around_save
##### before_create
##### around_create
##### after_create
##### after_save
##### after_commit/after_rollback
### 2 Updating an Object
##### before_validation
##### after_validation
##### before_save
##### around_save
##### before_update
##### around_update
##### after_update
##### after_save
##### after_commit/after_rollback
### 3 Destroying an Object
##### before_destroy
##### around_destroy
##### after_destroy
##### after_commit/after_rollback
## ***Active Record Associations***
##### belongs_to
##### has_one
##### has_many
##### has_many :through
##### has_one :through
##### has_and_belongs_to_many
## ***Active Record Query Interface***
### ***1.Retrieving a Single Object***
##### find: Sử dụng phương thức find, bạn có thể truy xuất đối tượng tương ứng với khóa chính được chỉ định phù hợp với bất kỳ tùy chọn được cung cấp nào (báo lỗi khi không tìm thấy)
##### take: Phương thức Take lấy một bản ghi mà không có bất kỳ thứ tự ngầm nào(trả về nil khi không tìm thấy)
##### first: Phương thức đầu tiên tìm thấy bản ghi đầu tiên được sắp xếp theo khóa chính (mặc định) (trả về nil khi không tìm thấy)
##### last: Phương thức cuối cùng tìm thấy bản ghi cuối được sắp xếp theo khóa chính (mặc định)(trả về nil khi không tìm thấy)
##### find_by:The find_by method finds the first record matching some conditions
### ***2.Retrieving Multiple Objects in Batches***
##### find_each:Phương thức find_each lấy các bản ghi theo lô và sau đó đưa từng cái vào khối
##### batch_size: batch_size cho phép bạn chỉ định số lượng bản ghi sẽ được truy xuất trong mỗi lô, trước khi được truyền riêng cho khối
##### start: start cho phép bạn định cấu hình ID đầu tiên của chuỗi bất cứ khi nào ID thấp nhất không phải là ID bạn cần
##### finish: kết thúc cho phép bạn định cấu hình ID cuối cùng của chuỗi bất cứ khi nào ID cao nhất không phải là ID bạn cần. Điều này sẽ hữu ích, ví dụ, nếu bạn muốn chạy một quy trình hàng loạt bằng cách sử dụng tập hợp con các bản ghi dựa trên: start và: finish
##### find_in_batches: Phương thức find_in_batches tương tự như find_each
### ***3.Conditions***


