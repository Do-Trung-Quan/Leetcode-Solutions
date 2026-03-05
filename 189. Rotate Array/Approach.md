# **Intuition**

3 Cách:

- tính k + duyệt for k lần rotate, mỗi lần rotate 1 ptu cuối lên đầu=> **Time Complexity: O(n*k) | Space Complexity: O(1)**
- tính k + tạo 1 mảng clone k phần tử cuối của nums + duyệt vòng for đưa các ptu ở vị trí trước nums.length - k về cuối và đưa các ptu trong mảng clone vào các vị trí ở đầu nums.=> **Time Complexity: O(n) | Space Complexity: O(N)**
- **tính k + 3 bước reversal phục vụ rotate array (Sẽ đi vào chi tiết cách này)**

# **Approach**

- **Tính k:** k = k chia dư cho muns.length
- **tạo hàm reverse(mảng, index bắt đầu (st), index kết thúc (en))**:
    - đưa vào vòng while với điều kiện (st < en):
        - swap nums[st] và nums[en]
        - cập nhật st++ và en--
- **thực hiện reverse nums + reverse đoạn trước k của nums + reverse đoạn sau k của nums**

# **Complexity**

- Time complexity: O(N), n là độ dài của nums
- Space complexity: O(1)
