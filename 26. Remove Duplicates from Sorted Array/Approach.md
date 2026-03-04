Intuition

Sử dụng 2 con trỏ và duyệt lần lượt trên nums để đưa các phần tử unique sang hết bên trái

Approach

Sử dụng 2 con trỏ:

- p = 1: con trỏ chỉ tới vị trí tiếp theo lưu phần tử unique

- i = 1: con trỏ của vòng lặp duyệt lần lượt từ đầu về cuối

Xử lý vòng lặp:

- So sánh nums[i] và nums[p-1] (nums[p-1] là phần tử unique thêm vào gần nhất):

- Nếu nums[i] != nums[p-1]: đưa phần tử nums[i] vào nums[p], cập nhập p++

Trả về p và mảng nums có p phần tủ đầu unique theo đúng order in-place

Complexity

Time complexity: O(n), n làm số ptu của nums

Space complexity: O(1)
