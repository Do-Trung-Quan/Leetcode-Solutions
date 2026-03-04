**Intuition**

Sử dụng 2 con trỏ và duyệt mảng đưa các phần tử khác val sang bên trái

1 con trỏ để xác định vị trí đưa phần tử, 1 con trỏ xác định phần tử hiện tại cần xét

**Approach**

Tạo 2 con trỏ:

- p = 0: con trỏ chỉ vị trí tiếp theo đưa phần tử sang

- i = 0: con trỏ chỉ index hiện tại đang xét trong vòng for

Xử lý vòng lặp:

- Nếu vị trí đang xét (nums[i]) khác val => đưa nums[i] vào vị trí p (nums[p]) và cập nhật p++

trả về p và mảng nums đã cập nhật p phần tử đầu tiên khác val

**Complexity**

Time complexity: O(n), n là độ dài nums

Space complexity: O(1)
