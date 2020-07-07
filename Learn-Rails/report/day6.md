# Chapter3 Mostly static pages
### Generrated static pages (Tạo trang tĩnh)
##### Generating a Static Pages controller.
##### *** $ rails generate controller StaticPages home help ***
##### Generate a model (tạo model)
##### *** $ rails generate model Tên-model tên-thuộc-tính: kiểu-dữ-liệu  *** 
### Migrations change the state of the database using the command (thay đổi trạng thái dữ liệu)
##### *** $ bundle exec rake db:migrate ***
##### Undo a single migration step using (Hoàn tác)
##### *** bundle exec rake db:rollback *** 
##### To go all the way back to the beginning, we can use (Quay về trạng thái ban đầu)
##### $ bundle exec rake db:migrate VERSION=0
##### assert_response(type, message = nil) 
##### :success - Status code was in the 200-299 range
##### :redirect - Status code was in the 300-399 range
##### :missing - Status code was 404
##### :error - Status code was in the 500-599 range
##### assert_select(*args, &block) public
##### Một xác nhận chọn các yếu tố và thực hiện một hoặc nhiều bài kiểm tra đẳng thức.
##### An assertion that selects elements and makes one or more equality tests.
##### If the first argument is an element, selects all matching elements starting from (and including) that element and all its children in depth-first order.
##### If no element if specified, calling assert_select selects from the response HTML unless assert_select is called from within an assert_select block.
##### When called with a block assert_select passes an array of selected elements to the block. Calling assert_select from the block, with no element specified, runs the assertion on the complete set of elements selected by the enclosing assertion. Alternatively the array may be iterated through so that assert_select can be called separately for each element.
##### <% provide %>