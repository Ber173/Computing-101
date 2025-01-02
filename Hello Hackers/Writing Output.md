# WRITE_UP

<img width="184" alt="Ảnh màn hình 2025-01-02 lúc 14 56 30" src="https://github.com/user-attachments/assets/a5a48f7b-584d-446f-9150-e9c4cbfba691" />

Explain:

    ; Gọi system call write
    mov rax, 1          ; Số syscall cho write
    mov rdi, 1          ; File descriptor (1 = standard output)
    mov rsi, 1337000    ; Địa chỉ của ký tự cần ghi
    mov rdx, 1          ; Số lượng ký tự cần ghi
    syscall             ; Thực hiện system call

    ; Thoát chương trình
    mov rax, 60         ; Số syscall cho exit
    xor rdi, rdi        ; Trả về mã thoát 0
    syscall             ; Thực hiện system call

 <img width="576" alt="Ảnh màn hình 2025-01-02 lúc 14 57 44" src="https://github.com/user-attachments/assets/ce7cc5e3-6993-4c2b-bd69-12f044e2d6ec" />
